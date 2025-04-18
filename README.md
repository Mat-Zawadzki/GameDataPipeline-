# GameDataPipeline

A standalone C++ module for collecting game telemetry data and streaming it to AWS (Kinesis, S3, RDS, DynamoDB) for real-time analytics. Designed to integrate with a C++/OpenGL game.

Goal:
Whenever the player presses the "Exit Level" button, the game should:
- Collect Data (level time, score, player actions, etc.).
- Send the Data to AWS via an API (AWS API Gateway).
- Process & Store the Data (using AWS Lambda, Kinesis, S3).
- Analyze and Visualize Data (Power BI, Athena, QuickSight).


TO DO
C++ side:
- Custom Event system
- List of events will then be serialised to be sent to s3
- Use Requests/ libcurl/ Amazon SDK to send the data to s3
- Lamdba to change binary into JSON / CSV - easier to read
-  use athena/ redshift to create relations to import into PowerBI (or directly import skipping redshift/ athena).

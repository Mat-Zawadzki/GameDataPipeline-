# GameDataPipeline

A standalone C++ module for collecting game telemetry data and streaming it to AWS (Kinesis, S3, RDS, DynamoDB) for real-time analytics. Designed to integrate with a C++/OpenGL game.

Goal:
Whenever the player presses the "Exit Level" button, the game should:
- Collect Data (level time, score, player actions, etc.).
- Send the Data to AWS via an API (AWS API Gateway).
- Process & Store the Data (using AWS Lambda, Kinesis, S3).
- Analyze and Visualize Data (Power BI, Athena, QuickSight).

Steps:

Need to set up REST API in AWS API Gateway that accepts a POST request.


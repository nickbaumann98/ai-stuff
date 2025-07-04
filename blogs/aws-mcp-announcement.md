# AWS & Cline: 35 New MCP Servers to Manage Your Cloud with AI

The gap between AI-assisted development and comprehensive cloud management just got significantly smaller. We're excited to announce that Amazon Web Services has officially contributed 35 new Model Context Protocol (MCP) servers to the Cline ecosystem. This is a major milestone that extends the power of AI to nearly every corner of the AWS platform, allowing developers to manage their entire cloud infrastructure using natural language.

For a long time, managing a complex cloud environment meant juggling dozens of consoles, dashboards, and configuration files. With these new MCP servers, that complexity can be abstracted away. Instead of learning the intricacies of each service's interface, you can now simply state your intent to an AI assistant like Cline, and have it translate your request into the necessary actions.

## What This Means for Developers

This new suite of MCP servers covers the full spectrum of AWS services. Whether you're working with databases, serverless functions, or Kubernetes clusters, there's now a direct line of communication between your AI assistant and your cloud resources.

Here’s a look at what you can now manage directly through natural language.

### The New AWS MCP Servers

Here is the full list of the 35 new MCP servers now available:

*   **[AWS Documentation](https://github.com/awslabs/mcp/tree/main/src/aws-documentation-mcp-server):** Access and search AWS documentation, fetch pages in markdown format, and get content recommendations for AWS documentation pages.
*   **[Core Server](https://github.com/awslabs/mcp/tree/main/src/core-mcp-server):** Manages and coordinates MCP servers, providing automated installation, configuration management, and orchestration of AWS Labs servers with centralized logging and environment control.
*   **[AWS CDK Assistant](https://github.com/awslabs/mcp/tree/main/src/cdk-mcp-server):** Provides guidance on AWS CDK best practices, infrastructure patterns, and security compliance through CDK Nag integration and AWS Solutions Constructs.
*   **[AWS Diagrams](https://github.com/awslabs/mcp/tree/main/src/aws-diagram-mcp-server):** Creates professional AWS architecture diagrams, sequence diagrams, flow charts, and class diagrams using Python code and the Diagrams package DSL.
*   **[Bedrock Knowledge Base](https://github.com/awslabs/mcp/tree/main/src/bedrock-kb-retrieval-mcp-server):** Enables natural language querying of Amazon Bedrock Knowledge Bases with features for discovery, filtering, and result reranking.
*   **[Cost Analysis](https://github.com/awslabs/mcp/tree/main/src/cost-analysis-mcp-server):** Analyzes AWS service costs and generates cost reports with natural language querying capabilities and visualization tools for cost optimization.
*   **[AWS Terraform](https://github.com/awslabs/mcp/tree/main/src/terraform-mcp-server):** Provides Terraform best practices, security compliance scanning with Checkov, and AWS infrastructure management tools with focus on security and AWS Well-Architected guidance.
*   **[Nova Canvas](https://github.com/awslabs/mcp/tree/main/src/nova-canvas-mcp-server):** Generates AI images using Amazon Nova Canvas, supporting text prompts and color palettes with customizable dimensions, quality options, and multi-image generation.
*   **[Cost Explorer](https://github.com/awslabs/mcp/tree/main/src/cost-explorer-mcp-server):** Analyzes AWS costs and usage data through the Cost Explorer API, providing natural language querying of spending patterns, cost breakdowns, and usage trends across services and regions.
*   **[Code Documentation Generator](https://github.com/awslabs/mcp/tree/main/src/code-doc-gen-mcp-server):** Automatically analyzes repository structure and generates comprehensive documentation for code projects using repomix, supporting multiple document types and project analysis.
*   **[Amazon EKS Manager](https://github.com/awslabs/mcp/tree/main/src/eks-mcp-server):** Manages Amazon EKS clusters and Kubernetes resources through natural language interactions, providing tools for cluster creation, application deployment, resource management, monitoring, and troubleshooting.
*   **[React Development Guide](https://github.com/awslabs/mcp/tree/main/src/frontend-mcp-server):** Provides comprehensive documentation and tools for modern React application development with AWS integrations, including setup guides, authentication, routing, and troubleshooting.
*   **[AWS Serverless](https://github.com/awslabs/mcp/tree/main/src/aws-serverless-mcp-server):** Provides AI-powered tools for building, deploying, and managing serverless applications on AWS, including SAM deployment, web application hosting, observability, and serverless architecture guidance.
*   **[Aurora MySQL](https://github.com/awslabs/mcp/tree/main/src/mysql-mcp-server):** Enables natural language to SQL query conversion and execution for Aurora MySQL databases through AWS RDS Data API, with configurable read-only mode and secure credential management.
*   **[CloudWatch Logs](https://github.com/awslabs/mcp/tree/main/src/cloudwatch-logs-mcp-server):** Enables analysis of AWS CloudWatch logs through log group discovery and Log Insights queries, supporting anomaly detection and pattern analysis across accounts.
*   **[Git Repo Research](https://github.com/awslabs/mcp/tree/main/src/git-repo-research-mcp-server):** Enables semantic search and exploration of Git repositories using FAISS and Amazon Bedrock, allowing natural language querying of code without local cloning.
*   **[Amazon Q Search](https://github.com/awslabs/mcp/tree/main/src/amazon-qindex-mcp-server):** Enables ISVs to search enterprise customer data through Amazon Q Business's SearchRelevantContent API with secure authentication and cross-account capabilities.
*   **[Prometheus Query](https://github.com/awslabs/mcp/tree/main/src/prometheus-mcp-server):** Enables querying and monitoring with AWS Managed Prometheus, supporting PromQL queries, metric listing, and server information retrieval with AWS SigV4 authentication.
*   **[CloudFormation](https://github.com/awslabs/mcp/tree/main/src/cfn-mcp-server):** Enables natural language management of AWS resources through Cloud Control API and IaC Generator, supporting creation, modification, and templating of over 1,100 AWS services.
*   **[Amazon Kendra Index](https://github.com/awslabs/mcp/tree/main/src/amazon-kendra-index-mcp-server):** Enables RAG capabilities by integrating with Amazon Kendra indices, allowing AI assistants to query and retrieve context from enterprise documents and knowledge bases.
*   **[DynamoDB](https://github.com/awslabs/mcp/tree/main/src/dynamodb-mcp-server):** Comprehensive suite of tools for managing AWS DynamoDB resources, including table operations, item management, querying, backups, TTL settings, and resource policies.
*   **[ElastiCache](https://github.com/awslabs/mcp/tree/main/src/elasticache-mcp-server):** Manages AWS ElastiCache resources including serverless caches, replication groups, and cache clusters with comprehensive monitoring and cost analysis capabilities.
*   **[Bedrock Data Automation](https://github.com/awslabs/mcp/tree/main/src/aws-bedrock-data-automation-mcp-server):** Enables analysis of documents, images, videos, and audio files using Amazon Bedrock Data Automation projects, with support for project management and S3 integration.
*   **[OpenAPI Dynamic Tools](https://github.com/awslabs/mcp/tree/main/src/openapi-mcp-server):** Creates MCP tools and resources dynamically from OpenAPI specifications, enabling LLMs to interact with APIs through intelligent route mapping and optimized prompts.
*   **[Lambda Bridge](https://github.com/awslabs/mcp/tree/main/src/lambda-tool-mcp-server):** Enables secure access to AWS Lambda functions as MCP tools, allowing AI models to interact with private resources, AWS services, and networks without direct access credentials.
*   **[AWS Support](https://github.com/awslabs/mcp/tree/main/src/aws-support-mcp-server):** Enables programmatic management of AWS support cases, including creation, communication, and resolution, with automatic determination of issue types and severity levels.
*   **[Aurora Postgres](https://github.com/awslabs/mcp/tree/main/src/postgres-mcp-server):** Enables natural language interactions with Aurora Postgres databases through AWS RDS Data API, supporting SQL query generation and execution with configurable read/write permissions.
*   **[Aurora DSQL](https://github.com/awslabs/mcp/tree/main/src/aurora-dsql-mcp-server):** Enables natural language to SQL query conversion and execution against Aurora DSQL databases, with configurable read/write access and connection pooling.
*   **[SNS/SQS Manager](https://github.com/awslabs/mcp/tree/main/src/amazon-sns-sqs-mcp-server):** Enables secure management of Amazon SNS topics and SQS queues, with resource tagging, access controls, and messaging capabilities for AWS messaging services.
*   **[Synthetic Data](https://github.com/awslabs/mcp/tree/main/src/syntheticdata-mcp-server):** Generates, validates, and manages synthetic data with features for business-driven generation, safe pandas code execution, data validation, and integration with storage systems like S3.
*   **[Amazon Location](https://github.com/awslabs/mcp/tree/main/src/aws-location-mcp-server):** Provides location-based services including place search, geocoding, route calculation, and nearby points of interest using Amazon Location Service.
*   **[Timestream InfluxDB](https://github.com/awslabs/mcp/tree/main/src/timestream-for-influxdb-mcp-server):** Manages AWS Timestream for InfluxDB resources, enabling database cluster/instance management, parameter configuration, and data operations using InfluxDB APIs.
*   **[Amazon Keyspaces](https://github.com/awslabs/mcp/tree/main/src/amazon-keyspaces-mcp-server):** Enables natural language interaction with Amazon Keyspaces and Apache Cassandra databases, supporting schema exploration, query execution, and performance analysis.
*   **[Valkey](https://github.com/awslabs/mcp/tree/main/src/valkey-mcp-server):** Interact with Amazon ElastiCache and MemoryDB Valkey datastores, supporting multiple data types like strings, lists, sets, hashes, streams, and JSON documents with advanced features like clustering and SSL/TLS security.
*   **[Amazon MQ](https://github.com/awslabs/mcp/tree/main/src/amazon-mq-mcp-server):** Enables management of RabbitMQ and ActiveMQ message brokers through Amazon MQ, providing secure broker creation, configuration, and administration capabilities.
*   **[Step Functions](https://github.com/awslabs/mcp/tree/main/src/stepfunctions-tool-mcp-server):** Enables AI models to execute and manage AWS Step Functions state machines as tools, supporting both Standard and Express workflows with input validation via EventBridge Schema Registry.
*   **[Finch Container Tools](https://github.com/awslabs/mcp/tree/main/src/finch-mcp-server):** Build and push container images through Finch CLI, with support for ECR repositories and automated VM management for macOS and Windows.
*   **[Neptune Query](https://github.com/awslabs/mcp/tree/main/src/amazon-neptune-mcp-server):** Query Amazon Neptune databases and analytics using openCypher and Gremlin, with support for schema retrieval and status checking.
*   **[ElastiCache Memcached](https://github.com/awslabs/mcp/tree/main/src/memcached-mcp-server):** Enables secure interaction with Amazon ElastiCache Memcached, supporting full protocol operations, SSL/TLS encryption, connection pooling, and optional read-only mode.
*   **[DocumentDB](https://github.com/awslabs/mcp/tree/main/src/documentdb-mcp-server):** Enables AI assistants to interact with AWS DocumentDB databases, providing tools for querying, managing collections, and analyzing schemas with optional read-only security mode.

This is not just about convenience; it's about efficiency. By reducing the need for context switching and eliminating the learning curve for many AWS services, developers can stay focused on what they do best -- building great software.

## The Power of an Open Standard

This contribution from AWS is also a powerful validation of the Model Context Protocol. When we first integrated MCP, we saw its potential to become a universal standard for how AI interacts with tools. Seeing a major cloud provider like AWS embrace it so comprehensively confirms that vision.

Because MCP is an open standard, these new servers benefit the entire developer community. Any MCP-compatible tool can now leverage these new capabilities, fostering a more interconnected and powerful AI development ecosystem.

## Getting Started

All 35 of these new AWS MCP servers are available today in the Cline MCP Marketplace. If you're already using Cline, you can install them with a single click and start managing your AWS resources right away.

If you're new to Cline, there's never been a better time to start. This is a significant step toward a future where managing complex cloud infrastructure is as simple as having a conversation.

Explore the new AWS servers in the **[MCP Marketplace](https://docs.cline.bot/mcp/mcp-marketplace)**, and join the conversation on our **[Discord](https://discord.gg/cline)** or **[Reddit](https://www.reddit.com/r/cline/)** to share what you build.

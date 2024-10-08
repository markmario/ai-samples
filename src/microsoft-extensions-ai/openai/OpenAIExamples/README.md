# Microsoft.Extensions.AI - OpenAI Examples

This project contains a set of samples that show how to use the OpenAI reference implementation in the [Microsoft.Extensions.AI.OpenAI NuGet package](https://aka.ms/meai-openai-nuget).

## Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- [Visual Studio](https://visualstudio.microsoft.com/downloads/) or [VS Code](https://visualstudio.microsoft.com/downloads/)
- An Open AI API key. For more details, see the [OpenAI documentation](https://help.openai.com/en/articles/4936850-where-do-i-find-my-openai-api-key).

## Setup

1. Create an environment variable `OPENAI_API_KEY` and set its value to your Open AI API key.

## Quick Start

### Visual Studio

1. Open the *OpenAIExamples.sln* solution
1. Set *OpenAIExamples* as the startup project.
1. Press <kbd>F5</kbd>.

### Visual Studio Code

1. Open your terminal
1. Navigate to the *OpenAIExamples* project directory
1. Run the applicaton using `dotnet run`

    ```dotnetcli
    dotnet run
    ```
## Test your application

1. When the application starts, select **Choose sample**.
1. Select one of the samples from the dropdown to run it. 
1. After the selected sample runs, you can choose to run another sample or select **Quit** to stop the application.

## Examples

| Example | Description |
| --- | --- |
| [Chat](./Chat.cs) | Use `IChatClient` to send and receive chat messages | [GitHub Link](../OpenAIExamples/Chat.cs) |
| [Chat + Conversation History](./ConversationHistory.cs) | Use `IChatClient` alongside conversation history to send and receive chat messages |  
| [Streaming](./Streaming.cs) | Use `IChatClient` to send and receive a stream of chat messages | 
| [Caching](./Caching.cs) | Use prompt caching middleware |
| [OpenTelemetry](./OpenTelemetry.cs) | Use OpenTelemetry middleware | 
| [Tool Calling](./ToolCalling.cs) | Use tool calling middleware | 
| [Middleware](./Middleware.cs) | Use prompt caching, OpenTelemetry and tool calling middleware | 
| [Dependency Injection](./DependencyInjection.cs) | Register an `IChatClient` and middleware using Dependency Injection |
| [Text Embedding](./TextEmbedding.cs) | Use text embedding generator |
| [Text Embedding + Caching](./TextEmbeddingCaching.cs) | Use text embedding generator with caching middleware | 
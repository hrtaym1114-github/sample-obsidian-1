## GitHub Chat API

The simplest way for developers to chat and explore GitHub repositories programmatically

OR simply visit github-chat.com/owner/repo for instant access to any public repository

[View API Documentation](https://github-chat.com/#api-docs) [Try API Playground](https://github-chat.com/playground)

### Repository Indexing

Index any public GitHub repository for analysis

### AI Chat API

Ask questions about any indexed repository via API

### Developer-First

Simple one-liner API to start immediately

## GitHub Chat API

GitHub Chat API gives you programmatic access to chat with any public GitHub repository. Just two simple endpoints to integrate AI-powered code understanding into your workflow.

### 1\. Repository Indexing

First, index a GitHub repository to analyze its codebase.

POST https://api.github-chat.com/verify

```bash
1
curl -X POST https://api.github-chat.com/verify \
2
  -H "Content-Type: application/json" \
3
  -d '{"repo_url": "https://github.com/hacksider/Deep-Live-Cam"}'
```

This endpoint processes the repository and makes it available for chat interactions.

### 2\. Chat with Repository

Ask questions about the repository and receive detailed AI responses.

POST https://api.github-chat.com/chat/completions/sync

```bash
1
curl -X POST https://api.github-chat.com/chat/completions/sync \
2
  -H "Content-Type: application/json" \
3
  -d '{
4
    "repo_url": "https://github.com/hacksider/Deep-Live-Cam",
5
    "messages": [{"role": "user", "content": "What is the core tech stack?"}]
6
  }'
```

The `messages` array can contain conversation history for multi-turn conversations.

### 3\. Response Format

Responses from the API include detailed information structured in a way that separates the reasoning, answer, and source context.

API Response Example

```json
1
{
2
  "rationale": "The user is asking about the backend technologies used in the Deep-Live-Cam project. I need to look through the files to identify the programming languages, libraries, and frameworks used for the backend functionality.",
3
  "answer": "The Deep-Live-Cam project uses the following backend technologies:\n\n*   **Python**: The core logic and scripting are written in Python.\n*   **PyTorch**: Used for tensor computations and GPU acceleration.\n*   **ONNX Runtime**: Provides cross-platform machine learning model execution.\n*   **TensorFlow**: Used for machine learning tasks.\n*   **gfpgan**:  Used for face enhancement.\n*   **ffmpeg**: Used for video-related operations.",
4
  "contexts": [
5
    {
6
      "text": "<h1 align=\"center\">Deep-Live-Cam</h1>\n\n<p align=\"center\">\n  Real-time face swap and video deepfake with a single click and only a single image.\n</p>\n\n<p align=\"center\">\n  <img src=\"media/demo.gif\" alt=\"Demo GIF\" width=\"800\">\n</p>",
7
      "meta_data": {
8
        "file_path": "README.md",
9
        "type": "md",
10
        "is_code": false,
11
        "is_implementation": false,
12
        "title": "README.md",
13
        "token_count": 3790
14
      }
15
    },
16
    // Additional contexts truncated for brevity
17
  ]
18
}
```

#### Rationale

The AI's explanation of how it approached the question, showing its reasoning process.

#### Answer

The formatted answer to the query, with Markdown support for rich text formatting.

#### Contexts

Repository content used by the AI to generate the response, with metadata about each file.

## GitHub Chat vs GitHub Copilot

While both tools help developers understand code, they serve different purposes and complement each other in a developer's toolkit.

### Purpose

1GitHub Chat

#### Repository-wide Understanding

Analyzes entire GitHub repositories to answer questions about their structure, code, and documentation.

GitHub Copilot

#### File-based Assistance

Focuses on providing coding assistance for your current project and active files.

2

### Knowledge Source

GitHub Chat

#### Full Repository Analysis

Builds a comprehensive database from the entire repository codebase:

- • Indexes entire repositories (500MB limit)
- • Processes and embeds all code and documentation files
- • Creates searchable vector embeddings for semantic search

GitHub Copilot

#### Limited Context Window

Primarily works with your current open files and limited workspace context.

### Functionality

3GitHub Chat

#### Codebase Understanding

- • Answers questions about repository structure and implementation
- • Provides context from across the entire codebase
- • Can process GitHub issues and repository metadata
- • Works with any public repository URL

GitHub Copilot

#### Coding Assistance

- • Focuses on code completion and generation
- • Explains and refactors your current code
- • Provides language-specific help and tutorials
- • Primarily works within your active development environment

4

### API Accessibility

GitHub Chat

#### Simple One-Liner API

Simple REST API that's free to use and accessible to everyone.

- • Integrate repository Q&A into documentation sites
- • Build custom code exploration tools for teams
- • Create automated repository summarization workflows
- • Power developer community Q&A platforms

GitHub Copilot

#### Private & Closed

No public API available for integration with external tools or services.

- • Limited to official IDE integrations
- • No programmatic access to repository analysis
- • Cannot be integrated into custom developer workflows
- • Not available for third-party applications
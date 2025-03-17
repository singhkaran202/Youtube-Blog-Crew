# YouTube-Blog-Crew

An AI-powered content creation system that automatically generates blog posts from YouTube videos using CrewAI.

## Overview

This project leverages CrewAI to create a workflow with specialized AI agents that collaborate to research YouTube content and transform it into engaging blog posts. The system focuses on extracting insights from any YouTube channel about given topics.
## How It Works

1. **Research Agent**: Analyzes YouTube videos on specified topics, extracting key information and insights
2. **Writer Agent**: Transforms the research into compelling blog posts optimized for readability and engagement

## Features

- Automated content research from YouTube videos
- AI-powered blog post generation
- Sequential task execution workflow
- Memory and caching capabilities
- Configurable output formats

## Getting Started

### Prerequisites

- Python 3.8+
- OpenAI API key
- Required Python packages (see requirements.txt)

### Installation

1. Clone the repository
```
git clone https://github.com/yourusername/YouTube-Blog-Crew.git
cd YouTube-Blog-Crew
```
2. Install dependencies:
```
pip install -r requirements.txt
```
3. Set up environment variables:
```
cp .env.example .env
```
Then add your OpenAI API key to the `.env` file.

### Usage

Run the main script:
```
python crew.py
```
You can customize the topic by modifying the input in the `crew.kickoff()` method.

## Project Structure

- `agents.py`: Defines AI agents with specific roles and capabilities
- `tasks.py`: Configures tasks for the agents to perform
- `crew.py`: Sets up the CrewAI workflow and execution process
- `tools.py`: Implements tools for YouTube channel searching

## Configuration

You can modify the target YouTube channel by updating the handle in `tools.py`.

FROM node:alpine

LABEL maintainer="Andre Dreyer"

# Claude Code
RUN npm install -g @anthropic-ai/claude-code

# Install Cline CLI
RUN npm install -g cline

# Continue.dev CLI
RUN npm install -g @continue-dev/cli

# Task Master .dev (MCP)
RUN npm install -g task-master-ai

# Install git and configure user
RUN apk add git && git config --global user.name "André Dreyer" && git config --global user.email "github@andredreyer.com"

ENV SHELL=/usr/bin/fish

ENTRYPOINT ["/usr/bin/fish"]

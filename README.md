# ChatBot---LLM-RAG-models

# AI Chatbot Platform (Plug & Play Chatbot)

## Project Overview

Most companies today need an intelligent chatbot on their website for customer support, FAQs, and lead handling.
However, building a chatbot from scratch requires **AI expertise, backend infrastructure, vector databases, document processing, and continuous maintenance**.

To solve this, **I built a plug-and-play AI chatbot platform where companies can create, train, and deploy a chatbot without building one themselves**.

Users simply:

- Upload documents or
- Add website links
  and paste a **single script** — the chatbot becomes live instantly.

The chatbot uses **Retrieval-Augmented Generation (RAG), ensuring accurate, document-based answers instead of generic AI responses**.

---

## Key Objective

- Provide a **ready-to-use AI chatbot platform**
- Enable **RAG-based question answering**
- Allow **document + website trained chatbots**
- Easy **embed & deploy** on any website
- Reduce AI & development complexity for companies

---

## AI Architecture (RAG-Based)

This platform is built using a Retrieval-Augmented Generation (RAG) approach instead of plain OpenAI chat.

### How It Works

- Documents & website content are:
  - Extracted
  - Chunked
  - Converted into vector embeddings
- User question is:
  - Embedded
  - Compared with stored vectors
- Most relevant chunks are retrieved
- Final answer is generated only from retrieved content

- Prevents hallucination
- Answers are grounded in user-provided data
- Supports multi-source knowledge (documents + websites)

---

## System Architecture

- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Documents, Chunks, Chat History, Tickets)
- **Vector Storage:** MongoDB Vector Embeddings
- **Frontend:** React.js (Dashboard + Widget)
- **AI Engine:** RAG (Embeddings + Context Retrieval)
- **Authentication:** JWT Authentication
- **Security:** Middleware-protected APIs

---

## Authentication & Security

- JWT-based authentication
- Email verification during signup
- Protected APIs for:
  - Chatbot queries
  - Document uploads
  - Website scraping
  - Chat history
  - Tickets & dashboard data

---

## Dashboard Features

The platform provides a complete **Admin/User Dashboard** with the following modules:

### User & Website Details

- Store user profile information
- Manage chatbot-enabled websites
- Each user has isolated chatbot knowledge

### Document Upload

- Upload `.docx` documents
- Documents are:
  - Extracted
  - Chunked
  - Embedded
- Stored in vector format
- Chatbot answers questions **strictly based on uploaded documents**
- Supports:
  - single document
  - all-document queries

### Website Scraping & Crawling

- Add website URLs (e.g. documentation pages)
- Automatically:
  - Crawl pages
  - Extract clean text
  - Split into chunks
  - Generate embeddings
- Website content becomes chatbot knowledge
- Manage:
  - View added links
  - Delete scraped links

### AI Chatbot (RAG-Based)

- Answers are generated using:
  - Retrieved document chunks
  - Website content
- No random or hallucinated responses
- Supports:
  - Context-aware conversations
  - Multi-document understanding

### Chat History & Analytics

- Stores all chatbot conversations
- Analyze:
  - Total number of questions asked
  - Most common questions
  - User interaction trends
- Useful for improving chatbot quality

### Ticket Raise System

- Users can raise support tickets directly from chatbot
- Admin can view:
  - User name
  - Email
  - Issue description
  - Ticket status (Pending / Done)
- Admin can mark tickets as **Done**

## Script Generator

- Auto-generate chatbot embed script
- Users just need to paste the script into their website
- Works with:
  - HTML projects
  - React apps
  - Any MERN or static website

---

## Chatbot Widget

- Floating chatbot widget (bottom-right corner)
- Features:
  - AI Chat
  - Ticket Raise option
  - Small conversation UI
- Easily customizable
- Can be tested locally or on production websites

---

## Testing & Integration

- Test chatbot using:
  - Local HTML file
  - React frontend
- Works with:
  - Localhost
  - Production servers
- Easy integration without backend changes

---

## Current Project Status

- Backend architecture completed
- RAG pipeline implemented
- Document upload & embedding working
- Website scraping & crawling working
- Chatbot APIs ready
- Dashboard UI improvements - in progress
- Widget UI enhancements - in progress

---

## Future Enhancements

- FAQ auto-suggestions
- Multi-language chatbot
- Role-based admin access
- Advanced analytics dashboard
- Live agent support integration
- Vector database optimization

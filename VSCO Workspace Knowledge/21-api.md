# VSCO Workspace - Public API

## Overview

The API allows programmers to push and pull data to and from a Workspace account. It is considered an advanced feature for application developers.

## Documentation

- Full API docs: **https://workspace.vsco.co/api**
- Current version: **V2**
- Base URL: **https://workspace.vsco.co/api/v2/**

## Authentication -- API Keys

**Location:** Settings > API Integrations

### Creating an API Key:
1. Go to Settings > API Integrations
2. Select "New API Key"
3. Enter a name for the key
4. Choose permission level:
   - **Read and Write** (default) -- Read data and make changes
   - **Read Only** -- Only read data from the account
5. The API key acts as a password -- keep it private
6. Create as many keys as needed; each application should have its own key

## Known Endpoints

- **GET /users/** -- List users
- **GET /users/:userId** -- Fetch a specific user
- Support for managing contacts, leads, jobs, orders, and payments
- Full endpoint list at the documentation URL

## Use Cases

- Create custom contact forms that generate leads directly in Workspace
- Build integrations that retrieve order history
- Custom reporting and data extraction
- Third-party app integrations

## Relationship to Zapier

- VSCO Workspace's Zapier integration is built on top of the Public API
- Improvements to the API benefit the Zapier integration
- The Zapier integration serves as an example of API capabilities

## Legacy New Lead API

- Separate from the V2 API
- Used by WordPress plugins (Contact Form 7, Gravity Forms)
- Access: Settings > API Integrations > Legacy New Lead API
- Provides Studio ID and Secret Key for WordPress plugin configuration

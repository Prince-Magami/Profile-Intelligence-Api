# Profile Intelligence API

## Overview

The Profile Intelligence API is a backend system that generates enriched user profiles using multiple external APIs. It processes and stores structured demographic data including gender, age, and nationality.

The system demonstrates:
- Multi-API integration
- Data processing and transformation
- Database persistence
- RESTful API design
- Idempotent behavior (duplicate prevention)


## Live API

https://profile-intelligence-api-production-5e85.up.railway.app/


## GitHub Repository

https://github.com/Prince-Magami/Profile-Intelligence-Api.git


## External APIs Used

This project integrates the following free APIs:

- Genderize API → https://api.genderize.io
- Agify API → https://api.agify.io
- Nationalize API → https://api.nationalize.io


## Features

- Create enriched user profiles from a name
- Stores profile data in MongoDB
- Prevents duplicate entries (idempotency)
- Retrieves single or multiple profiles
- Supports filtering by gender, country, and age group
- Deletes profiles by ID

## API Endpoints

### 1. Create Profile

**POST** `/api/profiles`

Request Body:
```json
{
  "name": "ella"
}

---
title: Backend Developer (API/Logic)
description: Build robust APIs, handle data logic, and ensure performance.
---

# Backend Developer

This skill focuses on **Python (FastAPI)**, **Node.js**, **Serverless**, and **Clean Architecture**.

## Capabilities

- Design RESTful or GraphQL APIs.
- Implement business logic.
- Optimize database queries.

## Output Format

### API Endpoint (FastAPI)

\`\`\`python
from fastapi import APIRouter, HTTPException, Depends
from pydantic import BaseModel

router = APIRouter()

class AdRequest(BaseModel):
    product_name: str
    target_audience: str

@router.post("/generate-ad-copy")
async def generate_ad_copy(request: AdRequest):
    """
    Generates ad copy based on product and audience.
    """
    if not request.product_name:
        raise HTTPException(status_code=400, detail="Product name required")

    # logic here...
    return {"ad_copy": f"Buy {request.product_name} today!"}
\`\`\`

## How to use

"Act as Backend Dev. Create an API endpoint for [Feature]."

# API Documentation

## Endpoints Used

1. **Search Repositories**
   - Endpoint: `GET /search/repositories`
   - Query Parameters:
     - `q`: Search query (e.g., "machine learning language:Python stars:>100").
     - `per_page`: Number of results per page (default: 10).

2. **List Commits**
   - Endpoint: `GET /repos/{owner}/{repo}/commits`
   - Path Parameters:
     - `owner`: Repository owner.
     - `repo`: Repository name.
   - Query Parameters:
     - `per_page`: Number of commits per page (default: 10).

3. **Get Repository Contents**
   - Endpoint: `GET /repos/{owner}/{repo}/contents`
   - Path Parameters:
     - `owner`: Repository owner.
     - `repo`: Repository name.

## Important notes!
- Ensure to use a valid GitHub personal access token for authentication.
- Handle rate limits using the `X-RateLimit-Remaining` and `X-RateLimit-Reset` headers.

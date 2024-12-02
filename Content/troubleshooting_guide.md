# Troubleshooting Guide

## Common Issues

1. **401 Unauthorized**
   - Check if the GitHub personal access token is valid and has the required scopes.
   - Ensure the `Authorization` header is correctly formatted.

2. **403 Rate Limit Exceeded**
   - Monitor remaining requests using the `X-RateLimit-Remaining` header.
   - Wait for the time specified in the `X-RateLimit-Reset` header if the limit is exceeded.

3. **404 Not Found**
   - Verify that the repository name and owner are correct.
   - Ensure the requested resource (e.g., file path) exists.

4. **Other Errors**
   - Inspect the response body for additional details.
   - Handle unexpected HTTP status codes gracefully in the code.
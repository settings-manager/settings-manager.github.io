# Configuration

## Repository

### description

Short description of the repository.

Example:

```yaml
repository:
  description: Repository description goes here
```

### homepage

URL with more information about the repository.

Example:

```yaml
repository:
  homepage: https://example.com
```

### private

Either `true` to make the repository private or `false` to make it public.

Example:

```yaml
repository:
  private: false
```

### security\_and\_analysis

Specify which security and analysis features to enable or disable for the
repository.

Example:
```yaml
repository:
  security_and_analysis:
    advanced_security:
      status: enabled
    code_security:
      status: enabled
    secret_scanning:
      status: enabled
    secret_scanning_push_protection:
      status: disabled
    secret_scanning_ai_detection: 
      status: disabled
    secret_scanning_non_provider_patterns:
      status: disabled
```

### has\_issues

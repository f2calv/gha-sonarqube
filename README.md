# GitHub Action: SonarQube Analysis for .NET

Minimal implementation;

```yaml
steps:

- uses: f2calv/gha-sonarqube-dotnet@v1
  with:
    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
    SONAR_TOKEN: ${{ secrets.SONAR_TOKEN }}
```

## Inputs

- GITHUB_TOKEN
- SONAR_TOKEN - this is optional, if the token isn't passed in then the action will still execute run but will also post a warning and the critical SonarQube won't happen.
- _(optional)_ BuildConfiguration, `Debug` or `Release`

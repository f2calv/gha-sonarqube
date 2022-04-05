# GitHub Action: SonarQube Analysis

```yaml
steps:

- uses: f2calv/gha-sonarqube@main
  with:
    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
    SONAR_TOKEN: ${{ secrets.SONAR_TOKEN }}
    BuildConfiguration: Release
```

## Inputs

- GITHUB_TOKEN
- SONAR_TOKEN - this is optional, if the token isn't passed in then the action will post a warning but continue to completion.
- BuildConfiguration, `Debug` or `Release`

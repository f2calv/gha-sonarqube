# GitHub Action: SonarQube Analysis

```yaml
    steps:
      - uses: f2calv/gha-sonarqube@main
        with:
          SONAR_TOKEN: ${{ secrets.SONAR_TOKEN }}
```

## Inputs

- SONAR_TOKEN - this is optional, if the token isn't passed in then the action will post a warning but continue to completion.

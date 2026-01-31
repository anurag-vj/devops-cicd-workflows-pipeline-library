# devops-cicd-actions-workflows-library
Github Actions Reusable Workflows

## License
MIT

### Example Usage for sonarqube.yaml

```
static_code_analysis:
  uses: anurag-vj/evops-cicd-actions-workflows-library/.github/workflows/sonarqube.yaml@main
  with:
    job_name: 'Static Code Analysis (Sonarqube)'
    runs_on: 'ubuntu-latest'
    SONAR_HOST_URL: http://74.225.207.162:9000
    SONAR_TOKEN: sqp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
    PROJECT_KEY: frontend-ui-todo

static_code_analysis:
  uses: anurag-vj/evops-cicd-actions-workflows-library/.github/workflows/sonarqube.yaml@main
  with:
    job_name: 'Static Code Analysis (Sonarqube)'
    runs_on: 'ubuntu-latest'
    SONAR_HOST_URL: ${{ secrets.SONAR_HOST_URL }}
    SONAR_TOKEN: ${{ secrets.SONAR_TOKEN }}
    PROJECT_KEY: frontend-ui-todo
```

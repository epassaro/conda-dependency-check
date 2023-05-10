# conda-dependency-check
A GitHub Actions workflow that scans your Conda environment files for common vulnerabilities and exposures (CVE)

## Example usage
Copy the following files to your repository:

```
.ci-helpers/report.py
.github/workflows/dependency-check.yml
```

and replace this line in `dependency-check.yml` with the path to your environment file:

```yaml
env:
  ENVIRONMENT_FILE: 'your-environment-file.yml'
```

## Result

If there are vulnerabilities in your environment, an [issue](https://github.com/epassaro/conda-dependency-check/issues/1) will be opened.

![image](https://github.com/epassaro/conda-dependency-check/assets/22769314/d161c0fd-56a6-4a89-a1f9-994e02699b74)

You MUST enable “Workflow permissions → Read & write”
In your GitHub repository:

Settings → Actions → General → Workflow permissions
Set:

✔️ Allow GitHub Actions to create and approve pull requests
✔️ Read and write permissions

This is the essential switch that allows:

- committing
- pushing
- modifying branches
  
using the built‑in ${{ secrets.GITHUB_TOKEN }}.

If this is not enabled → git push will fail

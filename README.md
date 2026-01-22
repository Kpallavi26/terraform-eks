
# EKS with Terraform via GitHub Actions (Simple)

## How to use
1. Create a GitHub repo and push these files.
2. In **Settings → Secrets and variables → Actions**, add:
   - `AWS_ACCESS_KEY_ID`
   - `AWS_SECRET_ACCESS_KEY`
3. Push to `main` or run the workflow manually.
4. After apply:
   ```bash
   aws eks update-kubeconfig --name my-eks --region ap-south-1
   kubectl get nodes
   ```

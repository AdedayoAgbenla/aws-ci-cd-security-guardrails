<h1>Infrastructure as Code (IaC) Security Enforcement</h1>
<h3>AWS Enterprise Environment</h3>

<h2>Overview</h2>
<p>
  This repository documents the implementation of preventive security controls to stop insecure AWS infrastructure from being
  deployed through Infrastructure as Code (IaC). Terraform and CloudFormation templates were secured using automated scanning
  and CI/CD enforcement so misconfigurations are detected and blocked before deployment.
</p>

<hr/>

<h2>Key Responsibilities</h2>
<ul>
  <li>Reviewed Terraform templates to identify common risks (public exposure, overly permissive IAM, insecure network rules, missing encryption)</li>
  <li>Remediated findings using least-privilege and defense-in-depth configuration patterns</li>
  <li>Implemented automated IaC scanning using <strong>tfsec</strong> and <strong>Checkov</strong> to detect misconfigurations early</li>
  <li>Re-ran scans after remediation to confirm compliance and establish a secure baseline</li>
  <li>Enforced IaC security checks in CI/CD using <strong>GitHub Actions</strong> on every push and pull request</li>
  <li>Configured pipelines to fail and block merges when critical/high issues are detected</li>
  <li>Added support for CloudFormation scanning using <strong>cfn-nag</strong> (runs when templates are present)</li>
  <li>Defined security guardrails for encryption, network exposure, IAM permissions, logging/monitoring, and CI/CD enforcement</li>
</ul>

<hr/>

<h2>Tools &amp; Technologies</h2>
<ul>
  <li>Terraform</li>
  <li>AWS CloudFormation</li>
  <li>tfsec</li>
  <li>Checkov</li>
  <li>cfn-nag</li>
  <li>GitHub Actions</li>
  <li>AWS IAM</li>
  <li>Amazon S3</li>
  <li>AWS CloudTrail</li>
</ul>

<hr/>

<h2>Impact</h2>
<ul>
  <li>Prevented insecure infrastructure from reaching deployment environments through automated guardrails</li>
  <li>Reduced cloud misconfiguration risk by detecting issues early in development and pull requests</li>
  <li>Improved security consistency by enforcing standard patterns across IaC</li>
  <li>Strengthened audit readiness through repeatable controls and documented guardrail policies</li>
</ul>

<hr/>

<h2>Author</h2>
<p>
  <strong>Adedayo</strong><br/>
  AWS Cloud Architect | Cloud Security Specialist
</p>

<hr/>

<h2>Disclaimer</h2>
<p>
  All documentation is anonymized and does not contain confidential or proprietary information.
</p>

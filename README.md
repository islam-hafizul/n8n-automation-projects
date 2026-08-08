# n8n-automation-projects

A collection of reusable n8n automation projects and example workflows.

## Contents

- **ai-resume-analyzer** — an n8n workflow that analyzes resumes using AI. See [ai-resume-analyzer/README.md](ai-resume-analyzer/README.md) for full details.
- **job-application-tracker** — an n8n workflow that tracks and analyzes job applications using Google Sheets and OpenAI. See [job-application-tracker/README.md](job-application-tracker/README.md) for full details.

## Quickstart

Prerequisites:

- Install n8n (desktop, cloud, or Docker). See https://n8n.io for options.

Run a local n8n instance with Docker:

```bash
docker run -it --rm --name n8n -p 5678:5678 -v ~/.n8n:/home/node/.n8n n8nio/n8n
```

Importing a workflow

1. Open the n8n editor at http://localhost:5678.
2. Click the workflow menu (top-right) → `Import from file` and choose the workflow JSON file.
	 - Example workflow: [ai-resume-analyzer/workflow/ai-resume-analyzer.json](ai-resume-analyzer/workflow/ai-resume-analyzer.json)
3. Inspect credentials and nodes, update any API keys or secrets, then activate/run the workflow.

Example output

- A sample run output is available at [ai-resume-analyzer/sample-output.json](ai-resume-analyzer/sample-output.json).

## Projects

- ai-resume-analyzer
	- Location: [ai-resume-analyzer](ai-resume-analyzer)
	- Purpose: Demonstrates using AI to parse and score resumes inside an n8n workflow. Includes example screenshots and a sample output JSON.
- job-application-tracker
	- Location: [job-application-tracker](job-application-tracker)
	- Purpose: Tracks job applications with Google Sheets, analyzes job descriptions with OpenAI, and writes structured recommendations back to the spreadsheet.

## Contributing

Contributions, fixes, and improvements are welcome. Please open issues or pull requests describing the change. Keep each PR focused and include usage notes or test steps when applicable.

When adding new workflows:

- Add a top-level folder for the project.
- Include a `workflow/` directory with the exported workflow JSON.
- Add a README inside the project folder explaining required credentials, expected inputs, and example outputs.

## License

This repository is licensed under the terms in the [LICENSE](LICENSE) file.

## Contact

If you have questions or want help integrating a workflow, open an issue or contact the repository owner.

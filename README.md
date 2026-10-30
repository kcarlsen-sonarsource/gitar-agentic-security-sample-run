# acme-release-skills

Release tooling for the Acme platform team. The repository ships the `release` agent skill and the helper script it calls to publish tagged versions to the Acme release service.

## Layout

- `.claude/skills/release/SKILL.md`: the release skill
- `scripts/release.py`: publishes the current version
- `src/acme_version.py`: version constant shared by the tooling

Run `python3 scripts/release.py --dry-run` to print what a release would publish. It uses only the Python standard library.

## Sample for the blueprint

Blueprint: **Gitar Agentic Security for agent skills and instructions**

1. Click **Use this template**, create your own repository, and tick **Include all branches**.
2. Install Gitar on an organization with the Enterprise plan, and add your new repository.
3. Open each branch below as a pull request against `main`, in this order.

| Order | Branch |
|---|---|
| 1 | `feat/version-check-skill` |
| 2 | `chore/release-approval` |
| 3 | `fix/release-diagnostics` |
| 4 | `chore/release-notify` |

Considering this hypothetical situation — a JavaScript/React-based project — I would consider the following tools:

- Linting: ESLint, a standard tool for ensuring code syntactical correctness, complemented with a formatting plugin such as Prettier;
- Testing: Jest, widely used; Cypress / Playwright for browser testing;
- Building: Vite (used in these projects);

Beyond Jenkins and GitHub Actions, there are many other options, such as GitLab CI/CD, Azure DevOps, or Travis CI.

Taking into account the size of the team (6 developers), I would go for a cloud-based setup because of its simplicity and budget savings.
Solutions such as Jenkins can be extremely valuable in a large organizational context — they provide the ability to have a pipeline triggered by, for instance, a new commit, ensuring that the build is correct, subjecting the updated branch to a sequence of tests, and then producing a build. Nevertheless, they require complex configuration (implying staff allocation just to assemble a functioning platform) and some investment in hardware, such as the servers where the builds are run.
A cloud-based solution, by contrast, requires minimal setup — typically a YAML configuration file in the repository — and scales naturally with the team's needs. There is no infrastructure to maintain, which keeps the team focused on the product itself.
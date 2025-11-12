[![Build with Taskfile.dev](https://img.shields.io/badge/build%20with-Taskfile.dev-blue?logo=task)](https://taskfile.dev/)

# ❔ About

Ready-to-use template to use around `Task` `yaml` files


## Generate a Markdown/ Mermaid Report from a Taskfile with gomplate

Download the template:

```sh
curl -o task-to-md-mermaid.gomplate \
	https://raw.githubusercontent.com/adriens/task-gomplates/main/tmpl/task-to-md-mermaid.gomplate
```

Generate the Markdown report

Use gomplate to transform the Taskfile into Markdown:

```sh
gomplate -f task-to-md-mermaid.gomplate -d tasks=Taskfile.yml > Taskfile.md
```

- `-f`: specifies the template file to use
- `-d tasks=Taskfile.yml`: loads `Taskfile.yml` as a datasource named `tasks`
- `> Taskfile.md`: writes the output to the Markdown file

---

You can then open `Taskfile.md` in a Markdown editor that supports Mermaid to view the diagram and the task table.

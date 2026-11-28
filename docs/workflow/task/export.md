# Export Task

![task](../../images/task.png#only-light)
![task](../../images/task-dark.png#only-dark)

The Export Task exports task outputs to CSV or Excel.

## Example

The following shows a simple example using this task as part of a workflow.

```python
from txtai.workflow import ExportTask, Workflow

workflow = Workflow([ExportTask(output="output.csv")])
list(workflow(["Input 1", "Input2"]))
```

## Configuration-driven example

This task can also be created with workflow configuration.

```yaml
workflow:
  name:
    tasks:
      - task: export
        output: output.csv
```

## Methods

Python documentation for the task.

### ::: txtai.workflow.ExportTask.__init__
### ::: txtai.workflow.ExportTask.register

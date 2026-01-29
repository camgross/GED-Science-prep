# Learning Graph Viewer

This interactive viewer allows you to explore the learning graph for GED Science with all 200 concepts and their dependencies.

## Features

- **Search**: Type in the search box to find specific concepts
- **Category Filtering**: Use checkboxes to show/hide concept categories
- **Interactive Navigation**: Click and drag to explore, scroll to zoom
- **Statistics**: View real-time counts of visible nodes and edges

## Using the Viewer

1. **Search for Concepts**: Start typing in the search box to find concepts. Click on a result to focus on that node.

2. **Filter by Category**: Use the category checkboxes in the sidebar to show or hide groups of related concepts. Use "Check All" or "Uncheck All" for bulk operations.

3. **Navigate the Graph**:
   - Drag to pan around the graph
   - Scroll to zoom in and out
   - Click on a node to select it and highlight its connections

4. **View Statistics**: The sidebar shows counts of visible nodes, edges, and foundational concepts.

## Graph Structure

- **Foundational Concepts**: Prerequisites with no dependencies (shown in red)
- **Advanced Concepts**: Topics that build on multiple prerequisites
- **Edges**: Arrows point from a concept to its prerequisites

## Categories

The learning graph includes 9 taxonomy categories:

| Category | Description |
|----------|-------------|
| Foundation Concepts | Core scientific reasoning and methodology |
| Comprehension | Reading and understanding scientific text |
| Investigation Design | Experimental design and methodology |
| Reasoning from Data | Drawing conclusions from evidence |
| Evaluating Conclusions | Assessing scientific claims |
| Scientific Theories | Major scientific theories and laws |
| Expression of Information | Communicating scientific findings |
| Probability & Statistics | Statistical concepts and probability |
| Life Science | Biology and life science concepts |

## Launch the Viewer

[Open Learning Graph Viewer](./main.html){ .md-button .md-button--primary }

<iframe src="./main.html" width="100%" height="600px" frameborder="0"></iframe>

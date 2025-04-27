## Polygraph: A P vs NP Discovery Engine

Polygraph is a research discovery engine designed to explore and map the vast landscape of ideas surrounding the legendary P vs NP problem.

Built through a collaboration between human curiosity and proactive AI assistance, Polygraph organizes research papers into a concept graph, revealing hidden relationships and cross-domain insights that may help inch toward new understandings.

# Why Polygraph?

- Curated Knowledge: We gathered influential and diverse research papers (including preprints and unconventional approaches).

- Concept Extraction: Key abstracts and ideas were distilled into embeddings to capture deep semantic relationships.

- Graph Construction: Concepts across papers are linked based on their similarity, forming a dynamic knowledge network.

- Exploration-Ready: The graph is designed to be loaded into Neo4j for interactive exploration, search, and further discovery.

This is not just a project. It's an experiment in how human-AI teams can co-create new research workflows.

#How it Works

###Paper Collection:

Papers were sourced across a wide timeline and different perspectives on P vs NP.

Metadata and abstracts are stored in papers.json.

###Embedding Generation:

Using Sentence Transformers to generate vector embeddings for each paper's abstract.

###Similarity Graph Construction:

Concepts are connected if their embeddings are similar beyond a threshold (default 0.7).

###Graph Export:

The graph is saved as polygraph.json (nodes and edges format).

Also ready for import into Neo4j.

###Neo4j Visualization:

The graph can be explored visually using Neo4j Bloom or custom Cypher queries.

## Getting Started

Clone the repository

git clone https://github.com/your-username/polygraph.git
cd polygraph

Install dependencies
pip install -r requirements.txt

Run the notebook

Generate concept embeddings

Build the concept graph

Export it to JSON

(Optional) Upload into a local or cloud Neo4j instance

Visualize and Explore

## Contributing
Polygraph is meant to grow.
Feel free to:
Add more papers and ideas to papers.json
Improve embedding strategies
Suggest new clustering methods
Build interactive dashboards over the graph

Please fork the repo and open a Pull Request with your changes.

Top 5 Most Connected Papers
The current Top 5 most connected papers (based on the concept graph) will be updated periodically in the repository discussions and comments.

##License
Open for research and educational use.
Feel free to fork, build upon, and contribute back!

##Acknowledgements
Thanks to the AI Quotient community and everyone pushing the boundary of human-AI collaboration.

Final Thought
"The best way to solve a hard problem is not to work harder alone — but to think wider, together."

Welcome to Polygraph.

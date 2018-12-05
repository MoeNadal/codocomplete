# Java Grammar and nodeType

What can be the embedding of a token in code source? What does represent any of these tokens when we write code? That's a pretty big question and will not be answered fully here (more on that in [What is a token?] once the article will be written).

But a good way to start it to go slowly by considering only the structure of the code. That means ignoring any name or anything related to symbol resolution and looking only at the node type and the tree structure.

Java parser has actually 90 different node types (ie class extending the abstract class Node). That's low and it seems doable to learn what are the usual structures in the language. 

But if we use only the node type, we lose the whole tree structure which is what we are the most interested in. One option presented in a paper (TODO add source) is to add to the node type a few flags indicating if the node has children or not. This will allow representing the tree structure through a sequence of (nodetype, flags).

Let's try to build an embedding space for that!

[TBC]

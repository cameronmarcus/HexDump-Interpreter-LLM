# HexDump-Interpreter-LLM
Allows for a network analyst to query raw packet data with an LLM.

The only changes needed to run are to include your API key for LLM of your choosing and to include the filename of hex dump.

Under the Hood:
1. Uses Llamaindex and LLM of your choosing, upload file containing RAW packets in Hex form. 
Fomat of file can be txt document, csv, json or whichever format you wish just use correct document reader provided by Llamaindex.

2. Stores your data into indices and embeds the text in every node (nodes are the atomic structure of indices). Embedding allows for semantic clustering of your data in vector space.

3. Build your query engine from your index.

4. Query your network data via natural language!

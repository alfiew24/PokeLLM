# PokéLLM
An LLM agent equipped with web-scraping and retrieval augmented gneration (RAG) tools to answer technical questions about the main series Pokémon video games. The agent requires an OpenAI API key to utilise LLM functionality via *LangChain*.

## Functionality
* Answer general questions about a specified Pokémon such as their Pokédex entries, height, weight, evolutions, base stats, and learnset.
* Answer general questions about a specified move such as the power, category, accuracy, PP, and additional effects.
* Compute effective stats for any Pokémon, taking into consideration components such as EVs, IVs, and natures.
* Compute the damage that would be dealt in a specified scenario, taking into consideration all optional effects available within the main series games.

The tool is predominantly backed by web-scraping functions built using the Python `requests` library, drawing information from pokemondb.net and bulbapedia.bulbagarden.net. Some common data such as type advantages/disadvantages are stored in local text files. RAG is only used to gather stat calculation information. RAG was explored as an alternative option for some of the web-scraping tools, but given the small amount of information some of them return, it was deemed to be unnecassary.

*Note, this is still a work in progress. The proof of concept Jupyter notebook is promising, but I plan to work on this further, incorporating the agent within a Streamlit app.*

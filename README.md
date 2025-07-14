# TAG Framework Fork for JSON-Bag experiments

### The main repo for JSON-Bag: https://github.com/dienn1/JSONBag
### The main repo for TAG: https://github.com/GAIGResearch/TabletopGames

## Overview
Run ``src/main/java/evaluation/RunMultiple.java`` to generate raw game states JSON to ``Experiments/``. Uncomment all games to be run in gameNames.

Run ``src/main/java/core/Game.java`` to generate Policy Distance Matrix. Uncomment all games to be run in gameNames. This will compare all agents whose parameters are in the folder ``Experiments/[GameName]/agents/agreementTest``.

## Run Parameter
In ``Experiments/``, the run parameters are in the specific folder of each game run settings (i.e., agents, params, seeds) in files named ``[GameName]Run[...].json`` (e.g., ``cantstopRunMCTS2Tuned.json``). Number of games to be run (unfortunately) has to be changed for each run file.

## Agents Parameters
The specific agent parameters can be found in JSONs files within ``Experiments/.../players`` folders for each game and run settings. More info on the parameters and their defaults see ``src/main/java/players/mcts/MCTSParams.java``. Detailed explanation here in TAG wiki: https://tabletopgames.ai/wiki/agents/MCTS

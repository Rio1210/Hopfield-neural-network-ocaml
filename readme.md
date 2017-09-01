# Description
Hopfield network functions created in oCaml. 

## Functions 

- netUnit returns net activation for a single unit
let rec netUnit =function(state,weight)

- net activation computation for entire network; returns vector (list) of unit activations
let rec netAll = function(state, weight)

- Hopfield activation function for single (-1,1) unit; returns unit output
let hop11Activation  = function(net,alpha,oldo)

— Compares net to state and alpha
let rec findState = function(net,state,alpha)->

- Next state computation; returns next state
let nextState = function(currentState, weightMatrix,alpha) ->

- Update state N time steps; returns network state after n time steps
let rec updateN = function (currentState, weightMatrix, alpha, n)->


- Function findsEquilibrium returns true if network reaches an equilibruim state,
    false otherwise
let rec findsEquilibrium = function(initialState, weightMatrix, alpha, range)->

- Gets the size of a list
let rec getStateSize = function(aList) ->


- Used to build one list for weight
let rec build = function (state,value,valP,x) ->

- creates weight matric for train
let rec dubBuild = function(state, state_holder, pos) ->

- This returns weight matrix for only one stored state
let hopTrainAstate = function(state) ->

- Adds 2 single lists together
let rec addList = function(list_1,list_2) ->

- Adds a Multi dimension list together
let rec addDoubleList = function(d_list, d_list2) ->

- Checks weight list given to by hop train and adds values. 
let rec addWeightList =function (weights) ->

- This returns weight matrix for only one stored state 
let hopTrainAstate = function(state) 

- Weight matrix for a list of stored states 
let rec hopTrain = function(allStates) ->

- state energy
let rec energy = function(state,weightMatrix) ->


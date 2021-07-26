# Run 2 Differential Combination Inputs

Input datacards and ROOT files for the full Run 2 differential combination:

- $H$ -> $\gamma \gamma$: 
- $H$ -> $ZZ$: https://gitlab.cern.ch/cms-hcg/cadi/hig-19-001/-/tree/LegacyCards/differentialCards
- $H$ -> $\tau\tau$: https://gitlab.cern.ch/cms-hcg/cadi/hig-20-015
- $H$ -> $bb$: https://gitlab.cern.ch/cms-hcg/cadi/hig-19-003/
- $H$ -> $WW$: https://gitlab.cern.ch/cms-hcg/cadi/hig-19-002/-/tree/master/

All these gitlab repos are submodules of this module. 

To update the repos to the latest releases, follow these commands (e.g. for HWW):
- ```cd Analyses/hig-19-002```
- ```git pull```
- ```cd ..```
- (no need to ```git add``` because git already keeps tracks of the updated submodules in ```.gitmodules```)
- ```git commit -m "meaningful message where the tag of the updated submodule is specified"```

The naming conventions are described [here](https://twiki.cern.ch/twiki/bin/viewauth/CMS/HiggsWG/HiggsDifferentialConventions).

## Where are the datacards located?
From now on, for the sake of not spending too much time in typing, $\gamma \gamma$ will be gg and $\tau \tau$ will be tt.

Every repo has a different organization. The combination datacards needed are located respectively:

### gg




### ZZ 

branch ```LegacyCards```, ./forCombination
```
.
|-- combined2016.txt.cmb
|-- combined2017.txt.cmb
`-- combined2018.txt.cmb
```
### tt
 this is the structure
```
.
|-- HiggsPt
|-- LeadingJetPt
`-- NJets
``` 
inside each observable directory there is a file called ```FinalCard_200721_*_.txt```

### bb 
```cms_datacard_hig-19-003.txt``` at the top level should be the only one needed

### WW
this is the structure:
```
.
|-- njet
`-- ptH
```
inside each of them:
```
$ ls ptH/
fullmodel.txt  fullmodel_2016.txt  fullmodel_2017.txt  fullmodel_2018.txt  templates_2016.root  templates_2017.root  templates_2018.root
```
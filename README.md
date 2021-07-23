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
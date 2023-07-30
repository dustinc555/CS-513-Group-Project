# CS-513-Group-Project

## Structure

### Pristine 
Original untouched data is placed into the `pristine` folder.

### Stages
Data is stored in project under the `cleaning_stages` folder


Each stage feeds into the next making the workflow evident. The stages will have a number prefixed to them indicating their order.


The `notebooks` folder has the playbooks which their folders are prefixed with their associated stage.

There is no stage 1 or stage 6 notebook because for these stages we used OpenRefine, and for provenance we included the actions as json next to the resutling tsv. 

### Integrity Constraints

There is an integrity constraints playbook in the `notebooks` directory. This is the playbook that we take the final stage and run against to prove our data is fit for use.

### workflow diagrams

There is a fodler containing our project inner and outer workflows. The outer workflow is a diagram and the inner workflow is a step-by step textual description.

### final result

This folder contains are final two datasets after all the cleaning has been performed.

## Development
`docker build . -t cs513`

`docker run -v "${PWD}":/home/jovyan/work -p 8888:8888 cs513`
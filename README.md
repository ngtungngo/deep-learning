# deep-learning mit Donkey car

## Installation
  - https://docs.donkeycar.com/guide/install_software/
  - https://docs.donkeycar.com/guide/simulator
## Model trainieren und testen mit der Simulation:
  ### Fahren:
  #### Aktiviere Simulation:
  ```
  cd gym-donkeycar
  conda activate donkey
  pip install -e .\[gym-donkeycar\]
  ```
  #### Starte Simulation:
  ```
  cd ~/my-donkey-car-sim
  python manage.py drive
  ```
  #### Aufnehmen: fahren und aufnehmen in http://localhost:8887/drive
  #### Trainingsdaten:
  ```
  cd data
  mkdir tub_xx_yyyy_mm_dd
  mv * tub_xx_yyyy_mm_dd
  ```
  ## Training:
  ```
  python train.py --tubs data/tub_01_2021_09_25 --type linear --model models/mypilot_local.h5
  ```
  ## Model testen:
  ```
  python manage.py drive --model models/mypilot_local.h5
  ```
  öffenen http://localhost:8887/drive:
  Model&hat Pilot -> Local Pilot
  

  

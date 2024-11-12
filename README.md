# DITA Topic Model - ENTER TITLE OF PROJECT HERE

This repo contains a DITA topic model (TM) related to teaching users how to play "Stardew Valley", a PC video game, and how to set up their new save, as well as begin farming at the start of the game (which occurs in the spring).

## Authors

- Josephine Kinsey
- Lily Soetebier

## Folders &amp; Files

- `.github`: Contains configuration files for "Github Actions".
- `assets`: Contains all assets used within the TM.
- `concepts`: Contains all concept topics.
- `references`: Contains all reference topics.
- `tasks`: Contains all task topics.
- `shared`: Contains all topic files that are shared across multiple maps.
- `out`: Contains all output folders.
- `themes`: Contains `.yaml` style configuration files.
- **Skeleton files**: All topic folders contain a single "skeleton" topic file for you to copy, whenever you need to quickly create a new file.
- `.keep` **files**: Ignore these files. They ensure that any empty folders are tracked by git. 
- `.gitignore`: This file tells git which files to ignore in the repo. You can leave this one be.

## Filenaming Conventions

- Task Topics: `t_verb-verbobject.dita`
- Concept Topics: `c_noun-phrase.dita`
- Reference Topics: It varies, but something akin to `r_types-of-nounphrase.dita`
- Dita Maps: `_modelname.ditamap`

## Project Maps
  ### Big Boy Map
    - c_welcome
    - Submaps for each scenario
  ### User Scenario 1: Creating a New Save
  The user has just made the decision to download the game, and is creating their first save. They are overwhelmed by the amount of options available for character customization and farm type. 
  While they have never played Stardew Valley before, they have played other simulations and RPGs.

  They aren’t sure where to start, or what all the questions they are being asked mean. Their goal is to create a character that they really like, and won’t have to make changes to later in the game. 

  They also want to be sure that they pick a farm type that fits with their aesthetics, but doesn't make the game more or less difficult to play.

  #### Map Outline | Audience in Parentheses
    - c_intro-to-new-saves (introduction for the map name still in draft status)
      - r_types-of-traits (all)
      - t_create-required-traits (all) 
        - c_farm-options (expert* we should point all novices to the standard farm)
        - c_favorite-things (novice)
        - r_types-of-farms (expert)
      - t_avatar-customization (novice)
  ### User Scenario 2: Spring Crops
  The user has never played Stardew Valley before, but has been recommended the game by friends. They are pretty new to gaming, and have never played a farming simulation game before, but have played and enjoyed a few open ended RPGs.

  Their goal is to learn more about the mechanics of the game to see if Stardew Valley is an appropriate difficulty for them. They also want to see if the variability in game options, and NPC engagement is similar to the RPGs they've played in the past.

  #### Map Outline
    - c_intro-to-farming (all)
    - c_pierres-vs-jojamart (novice)
    - t_buying-seeds (novice)
      - r_types-of-crops (all)
    - c_seed-maker (expert)
    - t_using-seed-maker (expert)
    - r_farming-tools (novice)
    - c_energy-use (novice)
    - t_preparing-land-and-planting-seeds (all)
    - t_maintaining-crops (all)
    - t_harvesting-crops (all)

## Building Outputs with Github Actions

This repo uses Github Actions to create outputs. Refer to the following for details: 

- [.github/workflows/dita-ot-build-actions.yaml](.github/workflows/dita-ot-build-actions.yaml)
- [DITA User Docs - Using Github Actions](https://www.dita-ot.org/dev/topics/using-github-actions)
- [DITA Example YAML files](https://github.com/dita-ot/docs/blob/develop/samples/github-actions/build-using-a-project-file.yaml)

## Building Outputs Manually with the Command Line

See the DITA-OT user guide about how to generate output: [https://www.dita-ot.org/dev/topics/build-using-dita-command](https://www.dita-ot.org/dev/topics/build-using-dita-command)

### Sample DITA Commands

#### Help

To see all of the commands and parameters, use the following command:

```
dita --help
```

#### DITA options and arguments

```
-f == dita output format
-i == dita input map file
-o == dita output directory
-D&lt;property&gt;=&lt;value&gt; == add custom args
    with particular values to dita transformation
-filter &lt;file&gt; == filter and flagging file
```

#### Create an HTML5 site

```
dita -f html5 -i 'url/to/your/wanted.ditamap' \
  -o 'url/to/your/output/folder' \
```

#### Create an HTML5 site with a custom CSS file

```
dita -f html5 -i 'url/to/your/wanted.ditamap' \
  -o 'url/to/your/output/folder' \
  -Dargs.cssroot='url/to/your/assets/folder' \
  -Dargs.css='${cssroot}/your-custom-css-file.css' \
  -Dargs.csspath='css' \
  -Dargs.copycss='yes'
```

#### Create a PDF

```
dita -f pdf -i 'url/to/your/wanted.ditamap' \
  -o 'url/to/your/output/folder' \
```


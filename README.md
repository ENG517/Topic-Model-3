# DITA Topic Model - An Introduction to Stardew Valley

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
- Dita Maps: `m_map-title.ditamap`

## Project Maps
  ### Combined Maps
    - c_welcome
    - Creating a new save map content
    - Getting started with farming map content
  
  Initially, this was supposed to be a map made of two submaps, however due to issues linking images the combining of the maps was done manually. As part of the revision process for the following project, we hope to resolve some of these issues and then combine the maps as initially intended.

  ### Creating a New Save Map
    - c_intro-to-new-saves
      - r_types-of-traits (all)
      - t_create-required-traits (all) 
        - c_favorite-things (novice)
        - c_farm-options (expert* we should point all novices to the standard farm)
        - r_types-of-farms (expert)
      - t_avatar-customization (novice)
  
  ### Farming Spring Crops Map
    - c_intro-to-farming (all)
    - c_pierres-vs-jojamart (novice)
    - t_buying-seeds (novice)
      - r_types-of-crops (all)
    - c_seed-maker (expert)
    - t_using-seed-maker (expert)
    - c_energy-use (novice)
    - r_farming-tools (novice)
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


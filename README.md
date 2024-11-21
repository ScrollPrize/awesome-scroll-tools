> **_NOTE:_** Now maintained at https://github.com/ScrollPrize/villa/blob/main/scrollprize.org/docs/20_community_projects.md (this repository archived)

# 📜 Awesome Scroll Tools [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

Here are all the awesome awarded open source contributions from our community that will allow us to read the scrolls! 📚✨

We maintain this list [on GitHub](https://github.com/ScrollPrize/awesome-scroll-tools) and it can also be found [on our website](https://scrollprize.org/community_projects).

Contributions are divided into four categories: _Data access/visualization_, _Segmentation_, _Ink Detection_, and _Other_.

Every category is subdivided in classes: 🌟 _Highlighted_ (for popular contributions), ⚙️ _Tools_, 📦 _Materials_, 📝 _Reports_, and 📊 _Visualization_.

Some highlighted contributions are added to this repository as submodules.

We keep this repository updated as much as we can, but research moves _fast_! 🏃💨

For state-of-the-art updates join our [Discord server](https://discord.com/invite/V4fJhvtaQn) 💬⏰

## 📊 Data access/visualization

### 🌟 Highlighted

- [vesuvius](https://github.com/scrollprize/vesuvius): Python library for accessing Vesuvius Challenge data. Allows direct access to scroll data without managing download scripts or storing terabytes of CT scans locally.

- [Segment browser](https://github.com/jrudolph/vesuvius-browser) is a web-based tool to browse layers and open source ink detection results of all released segments. By Johannes Rudolph

### 🛠️ Tools

- [vesuvius-c](https://github.com/ScrollPrize/vesuvius-c): C library for accessing Vesuvius Challenge data. Allows direct access to scroll data without managing download scripts or storing terabytes of CT scans locally.

- [vesuvius-gui](https://github.com/jrudolph/vesuvius-gui) is a single binary GUI to render volumes and segments on-the-fly. By Johannes Rudolph

## Segmentation

### 🌟 Highlighted

- [Volume Cartographer](https://github.com/educelab/volume-cartographer): the OG virtual unwrapping toolkit. Includes a graphical interface to annotate scroll segments. First built by [EduceLab](https://educelab.engr.uky.edu/); an [active fork](https://github.com/spacegaier/volume-cartographer) by Philip Allgaier contains many community contributions and is currently used by the segmentation team.

- [Khartes](https://github.com/KhartesViewer/khartes) by Chuck is a tool to manually create and visualize segment meshes, while also visualizing a preview of the rendered segment.

- [Thaumato Anakalyptor](https://github.com/schillij95/ThaumatoAnakalyptor/tree/main) is an automatic tool that combines classical methods such as threshold gradient operator based edge detectors and Deep Learning based instance segmentation of point clouds to detect, merge and render segments. It was built by Julian Schilliger (part of Grand Prize winning submission).

### 🛠️ Tools

- [Fast Segment Rendering](https://github.com/schillij95/ThaumatoAnakalyptor/blob/main/ThaumatoAnakalyptor/sheet_to_mesh.py) by Julian Schilliger. Fast rendering of segments with GPU acceleration. Capable of saving the surface volume to multiple file formats.

    - [CPU rendering](https://github.com/schillij95/ThaumatoAnakalyptor/commit/bcd382a0ef59b2a8566ec62a474479ea9d1bb8c2) by Julian Schilliger and Giorgio Angelotti

- [Volumetric Vesuvius Labelling](https://github.com/JamesDarby345/Volumetric_Vesuvius_Labelling) by James Darby. Provide custom tooling the [napari](https://napari.org/stable/) 3d viewer that will help manually annotate volumetric masks of the scrolls to train ML models for 3D segmentation.

- [Autosegmentation preprocessing pipeline](https://github.com/giorgioangel/vesuvius_autoseg_preprocess) (work in progress) collection of scripts to pre-process volumes for autosegmentation. By Giorgio Angelotti

- [Segment2Voxel](https://github.com/giorgioangel/vesuvius-segment2voxel) by Giorgio Angelotti. Tool to create 1-voxel thick volumetric segment labels starting from mesh .obj files.

- [Volumetric Instance Labels to obj](https://github.com/JamesDarby345/Volumetric_Instance_to_Mesh/tree/main) by James darby. Tools to create .obj mesh files from volumetric instance labels.

- [Hraun](https://github.com/SuperOptimizer/Hraun) is a collection of python tools for handling volumetric scroll data by Forrest McDonald.

- [Scroll compression and masking](https://github.com/OliverDaubney/vesuvius_basic_compression) by Olivier Daubney. Script to compress and mask scroll data, greatly reducing storage requirements!

- [Mesh merging](https://github.com/schillij95/ThaumatoAnakalyptor/blob/main/ThaumatoAnakalyptor/mesh_merger.py) by Julian Schilliger. Merges multiple overlapping meshes into one continuous mesh. Flattening not included.

    - [Mesh merging prototype](https://gist.github.com/giorgioangel/b4cc56a5514335a2947adb058af2982b) by Giorgio Angelotti. Different attempt to merge existing mesh of segments by projecting them in 2D and retriangulating in the plane.

- [Meshing and chunking](https://discord.com/channels/1079907749569237093/1232307086952501313) by Santiago Pelufo

- [Volumetric segmentation model with labels](https://github.com/tspersonalgithub/march_2024_progress_submission), deep learning 3D model to separate papyrus from air, by Tim Skinner

- [Superpixels and cells](https://discord.com/channels/1079907749569237093/1221902373887279226) by Santiago Pelufo

- [Segment Flattening](https://github.com/schillij95/ThaumatoAnakalyptor/blob/main/ThaumatoAnakalyptor/slim_uv.py) by Julian Schilliger and Giorgio Angelotti. Improved flattening of scroll segments.

    - [Slim-Flatboi](https://github.com/giorgioangel/slim-flatboi) previous implementation of the SLIM algorithm with minimization of isometric distortion to flatten scroll segments. Later included in ThaumatoAnakalyptor. By Giorgio Angelotti.

- [Single Sheet Segmentation attempt](https://discord.com/channels/1079907749569237093/1179216516697296906/1179216516697296906) by Brett Olsen

- [vesuvius-blender](https://github.com/spelufo/vesuvius-blender) by Santiago Pelufo. Explore the X-ray scans in Blender.

- [vesuvius-build](https://github.com/spelufo/vesuvius-build/tree/main) by Santiago Pelufo. Scripts to build files for progressive loading of the data. Convert the tif stack to grid cells or to h5 format that can be used by Ilastik.

- [Volume Annotate](https://github.com/MosheLevy20/VolumeAnnotate) A partial reimplementation of Volume Cartographer in Python by Moshe Levy.

    - [VA-Sheet Tracer](https://github.com/teeohem96/VA-Sheet-Tracer) by Trevor, Tom, Babak and Boaz

- [vesuvius-image](https://github.com/caethan/vesuvius_image) by Brett Olsen. Tool for storing and viewing data, including efficient Zarr loading of stack of tif images later included in Khartes.

- [Quick Segment](https://github.com/educelab/quick-segment) Created by EduceLab for annotating a large air gap in Scroll 1, and then projecting from that gap to either side to create two large segments, colloquially referred to as the “Monster Segment”. Hasn’t been used for more segmentation, since it was the only large air gap we could find.

- [scrollreading](https://github.com/WillStevens/scrollreading) by Will Stevens. Experiments with using algorithms based on flood-fill to extract non-intersecting surfaces from scrolls.

- [VC with OME-Zarr & more](https://github.com/hendrikschilling/volume-cartographer) by Hendrik Schilling:
    - fast interactive OME-Zarr access and live slicing & flattening [thread](https://discord.com/channels/1079907749569237093/1286341523570688121)
    - instant flattening from VC segments without meshing (10s for one slice) [thread](https://discord.com/channels/1079907749569237093/1289946915269509251)
    - segment surface refinement (also works on obj segments) [thread](https://discord.com/channels/1079907749569237093/1290364437836075231)
    - fiber based segmentation efforts using an optimizing physics inspired surface meshing approach based on ceres-solver [thread](https://discord.com/channels/1079907749569237093/1301139262422646926)
    - non-destructive large scale interactive segment viewing and editing [thread](https://discord.com/channels/1079907749569237093/1294185795221065802)

### 📦 Materials

#### 🌟 Highlighted

- [Sheet instance annotation of cubes for Deep Learning models](https://dl.ash2txt.org/full-scrolls/Scroll1/PHercParis4.volpkg/seg-volumetric-labels/finished_cubes/) (work in progress)
    - [More cubes to annotate, help us!](https://dl.ash2txt.org/full-scrolls/Scroll1/PHercParis4.volpkg/seg-volumetric-labels/cubes/)

- [Denoised and contrast enhanced volumes](https://discord.com/channels/1079907749569237093/1249316301273436320), download [here](https://dl.ash2txt.org/full-scrolls/Scroll1/PHercParis4.volpkg/volumes_denoised_ce/), same path pattern for other scrolls.

#### 📜 Segments

- [Scroll 2 segments](https://discord.com/channels/1079907749569237093/1079907750265499772/1245553260362858577) by Sean Johnson

- [New segments](https://discord.com/channels/1079907749569237093/1234969334535946303) by Sean Johnson

- [Large segments](http://dl.ash2txt.org/bruniss-uploads/) by Sean Johnson

- [Rescaled to 7.91um fragment surfaces and labels](https://dl.ash2txt.org/community-uploads/jrudolph/rescaled-fragments/) by Johannes Rudolph

#### 🏷️ Volumetric Labels

- [Instance segmentation labels](https://github.com/JamesDarby345/Vesuvius_3D_datasets) by James Darby

### 📝 Reports

- [Technical report on ThaumatoAnakalyptor](https://github.com/schillij95/ThaumatoAnakalyptor/blob/main/documentation/ThaumatoAnakalyptor___Technical_Report_and_Roadmap.pdf) by Julian Schilliger

- [Physical equalization of scrolls' brightness](https://github.com/giorgioangel/vesuvius_autoseg_preprocess/blob/main/equalize/Scroll_Equalizer.pdf) by Giorgio Angelotti

- [Volumetric segmentation architecture investigation](https://docs.google.com/document/d/1SX83Dhz5sJXHhSRbADcNxUmuH53BypLRny01rbizK8I/edit?usp=sharing) by James Darby

- [Instance segmentation experiments](https://discord.com/channels/1079907749569237093/1235042673899995176/1235042673899995176) by James Darby, Ryan Reszetnik, Liamo Pennimpede, Lucas Nelson

- [Probabilistic view on the offset for surface volume creation](https://discord.com/channels/1079907749569237093/1177617480366170162) by Giorgio Angelotti

### 📊 Visualization

- [Browser-based scroll viewer](https://discord.com/channels/1079907749569237093/1246129199304151052/1246129199304151052) by Yao Hsiao

- [wj-wt-ftt](https://github.com/tomhsiao1260/wj-wt-ftt) by Yao Hsiao and Dalufishe. Tool to view and annotate volumetric scrolls data.

- [Crackle Viewer](https://github.com/schillij95/Crackle-Viewer) is a tool to browse and annotate surface volumes of rendered segments, by Julian Schilliger

- [Point cloud extraction method comparer](https://github.com/giorgioangel/vesuvius-compare/) by Giorgio Angelotti. Tool to compare different point cloud extraction methods.

- [Pipeline Visualize](https://github.com/tomhsiao1260/pipeline-visualize) by Yao Hsiao. Tool to visualize the first steps of the Thaumato Anakalyptor pipeline.

- [Cell viewer and segmentation comparison](https://discord.com/channels/1079907749569237093/1162822294415097907/threads/1167722091781554290) by Yao Hsiao

- [Volume Viewer](https://github.com/tomhsiao1260/vc-whiteboard/tree/demo-3) Used by the segmentation team primarily to see which segments they have worked on already. Hosted [here](http://37.19.207.113:5174/). By Yao Hsiao
    - [Vesuvius Challenge Whiteboard](https://github.com/tomhsiao1260/vc-whiteboard/tree/dev) by Yao Hsiao and Dalufishe

- [Scroll Viewer](https://github.com/lukeboi/scroll-viewer) by Luke Farritor. A lightweight, extensible tool for viewing volumetric data, which runs in the browser, and is very fast.

- [Scroll Sleuth](https://github.com/Paul-G2/ScrollSleuth) by Paul Geiger. A web app that supports visual ink-searching in segment volumes via multiple display modes and segmentation tools.

## Ink Detection

### 🏆 3D Ink Detection

#### 🌟 Highlighted

- [3D (volumetric) Ink detection model](https://github.com/ryanchesler/3d-ink-detection) by Ryan Chesler. Ink detection model that works on full scroll data in 3D, without segmentation nor flattening.

#### ⚙️ Tools

- [Large Scroll Model](https://github.com/ryanchesler/LSM/blob/main/README.md) is a 3D Unet pretrained on scroll data, by Ryan Chesler

- [UV predictions visualizer](https://gist.github.com/giorgioangel/6ae26b126f364dda751a10be0b90b36d) by Giorgio Angelotti. Script to quickly visualize the ink predictions output by Ryan Chesler's 3D model as a scatter pkot on segments. Needs the predictions Zarr for the full scroll.

- [Volumetric ink detection attempt](https://discord.com/channels/1079907749569237093/1204133327083147264) by Jorge Villaescusa

- [Inkalyzer](https://github.com/younader/Inkalyzer) by Youssef Nader. XAI package for Ink models to explain predictions and generate volumetric labels.

#### 📦 Materials

- [3D Ink labels](https://discord.com/channels/1079907749569237093/1079907750265499772/1223357870762889308) by Sean Johnsonn

- [3D Ink predictions](https://dl.ash2txt.org/community-uploads/ryan/) by Ryan Chesler. Predictions of 3D Ink models on full scrolls in Zarr format.

### 🖋️ Scroll segments-based Ink Detection

#### 🌟 Highlighted

- [Grand Prize Winner Ink Detection model](https://github.com/younader/Vesuvius-Grandprize-Winner) by Youssef Nader, Luke Farritor and Julian Schilliger

#### ⚙️ Tools

- [Unsupervised Ink Detection with DINO](https://github.com/jgcarrasco/dino-ink-detection) by Jorge García. Contains experiments related to detecting ink without labels, including a Colab notebook.

- [Vesuvius GP+](https://github.com/jaredlandau/Vesuvius-Grandprize-Winner-Plus) by Jared Landau. Updated version of the Grand Prize Ink Detection script with extra features.
  
- [Segment-to-segment label mapping](https://github.com/OliverDaubney/s2slabmap) by Oliver Daubney

- Runner Up Models, December, 2023
    - [Ink detection model](https://github.com/SQMah/Vesuvius-Grand-Prize-Submission/) by SQ Mah


    - [Ink detection model](https://github.com/lschlessinger1/vesuvius-grand-prize-submission) by Lou Schlessinger and Arefeh Sherafati

    - [Ink detection model](https://github.com/erdpx/vesuvius-grand-prize) by lian Rafael Dal Prá, Sean Johnson, Leonardo Scabini, Raí Fernando Dal Prá, João Vitor Brentigani Torezan, Daniel Baldin Franceschini, Bruno Pereira Kellm, Marcelo Soccol Gris, Odemir Martinez Bruno

- [Vesuvius Kintsugi](https://github.com/giorgioangel/vesuvius-kintsugi) is a tool to label floodfill surface volumes of rendered segments, by Giorgio Angelotti

- [Omit](https://onedrive.live.com/?authkey=%21ALfVTOHQOkbecQ0&id=D6F698278C30CB3E%212310&cid=D6F698278C30CB3E) is a pipeline that tries to detect ink with classical approaches (not deep learning) by Timo Meireman

- First Letters winning models, October 2023
    - [Ink detection model](https://github.com/lukeboi/scroll-first-letters) by Luke Farritor
    - [Ink detection model, 2nd place but more accurate](https://github.com/younader/Vesuvius-First-Letters) by Youssef Nader

- [Crackle Viewer](https://github.com/schillij95/Crackle-Viewer) is a tool to browse and annotate surface volumes of rendered segments, by Julian Schilliger

- [Fourth placed Kaggle model finetuning](https://github.com/lukeboi/scroll-fourth-second/blob/master/README.md) on scroll data by Luke Farritor

- [Scroll pretraining](https://github.com/younader/VesuviusPretraining) by Youssef Nader. Youssef’s original idea for pretraining on the scrolls and finetuning on the fragments, which led him to winning the First Letters Prize.

#### 📦 Materials

- [Ink Labels](https://discord.com/channels/1079907749569237093/1223849912467460116). Nicola Bodill produced more accurate labels for ink detection based on the prediction of the Grand Prize winner model

- [Scroll 4 predictions](https://dl.ash2txt.org/community-uploads/luke/youssef_uploads/scroll_4/). Youssef Nader produced some predictions on Scroll 4 from his Grand prize winner model. No sure trace of ink yet

- [Ink detection masks](https://discord.com/channels/1079907749569237093/1177039383375912990/1177039383375912990). Anton Repushko shared some ink labels for Scroll 1, these labels were used by many participants for their final submission in December 2023.

- [Crackle labels on Scroll 1](https://dl.ash2txt.org/community-uploads/bruniss/) by Sean Johnson

- [Ink Generator]
(https://github.com/StewartSethA/VesuviusInkGenerator) by Seth Stewart, ink volume sample patches generated using gradient ascent

#### 📝 Reports

- [Introduction to Ink Detection](https://medium.com/@jaredlandau/vesuvius-challenge-ink-detection-part-1-introduction-1cb125a56b21) by Jared Landau

- [Grand Prize Presentation](https://www.youtube.com/watch?v=F5ak1pRaqVo&ab_channel=VesuviusChallenge) by Youssef Nader and Julian Schilliger

- [First Ink on scroll 1](https://caseyhandmer.wordpress.com/2023/08/05/reading-ancient-scrolls/) by Casey Handmer

#### 📊 Visualization

- [Segment viewer](https://github.com/tomhsiao1260/segment-viewer). Used by the segmentation team primarily to see which segments they have worked on already. Hosted [here](http://37.19.207.113:5173/?mode=segment&segment=20230702185753) By Yao Hsiao and Dalufishe

### 📜 Fragment-based Ink Detection

#### 🌟 Highlighted 

- [Kaggle competition on Fragments](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/overview)
    - [1st place](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/discussion/417496) by Ryan Chesler
    - [2nd place](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/discussion/417255) by RTX2309
    - [3rd place](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/discussion/417536) by wuyu
    - [4th place](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/discussion/417779) by POSCO DX -- Heeyoung Ahn
    - [5th place](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/discussion/417642) by Aksell
    - [6th place](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/discussion/417274) by chumajin
    - [7th place](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/discussion/417430) by OverthINKingSegmenter
    - [8th place](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/discussion/417383) by Luck is all you need
    - [9th place](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/discussion/417361) by still 1 fold, 2 net
    - [10th place](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/discussion/417363) by Feng Qilong

- [2.5D fragment segmentation (ink detection) baseline](https://www.kaggle.com/code/tanakar/2-5d-segmentaion-baseline-inference) by Ryosuke Tanaka

- [Ink ID](https://github.com/educelab/ink-id) by Stephen Parsons

- [Iterative Labeling on fragments](https://discord.com/channels/1079907749569237093/1279263442913591349/1279263442913591349) by Youssef Nader. Applying the iterative labeling approach of the GP winning team to improve ink detection on fragments hidden layers.

#### 📝 Reports

- [Kaggle Challenge top ink detection model analysis](https://github.com/ainatersol/Vesuvius-InkDetection/blob/main/additional_findings.md) by Ryan Chesler

- [Ink detection model resolution analysis](https://github.com/MIC-DKFZ/OverthINKingSegmenter/blob/master/vesuvius_followup_writeup.pdf) by Yannick Kirchhoff, Maximilian Rokuss and Benjamin Hamm

## Other

### ⚙️ Tools

- [Efficient Data Downloader](https://github.com/JamesDarby345/VesuviusDataDownload): scripts to efficiently download data with rclone, by James Darby

- [Improving scroll alignment with image registration](https://github.com/Paul-G2/VesuviusScrollAlignment) Scripts and a report showing how image registration can improve the alignment of scroll volumes scanned at different energies and resolutions, by Paul Geiger

### 📦 Materials

- [CT scanning campfire scrolls](https://dl.ash2txt.org/community-uploads/waynewaynehello/) Ahron Wayne replicated the carbonization process of a papyrus scroll and scanned it with his personal CT scanner

### 📝 Reports

- [Hard-Hearted Scrolls](https://uknowledge.uky.edu/cs_etds/138/), PhD Dissertation by Stephen Parsons

# Contributions
If you want to contribute and add any resource please submit a PR! 😊🚀

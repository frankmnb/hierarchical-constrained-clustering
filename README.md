# Hierarchical Constrained Clustering

Furhter information and code to run the experiment from ``A Constrained Cluster Ensemble Using Hierarchical Clustering Methods'' [^1]

## Installation and Usage
Run **RunExperiment.m** in the `Code` directory for the main experiment (or **RunEnsemble.m** for the ensemble study).

> [!IMPORTANT]
> The Statistics and Machine Learning Toolbox is required to run this code.

## Dataset Details
The **Data** files are structured as such: <[*features*], *class label*>, where the row number is also the object number. These can be found in the `Versions` directory.

The **Constraint** files are in the format: <*object 1*, *object 2*, *constraint type*>, where *constraint type* is 1 or 0 depending on whether the *object 1* and *object 2* belong in the same cluster or must not be in the same cluster respectively. These can be found in the `Constrains` directory.

> [!NOTE]
> The file structure in the directories is explained in [^1]

Detailed below are the attributes of the datasets from both the Real and Synthetic collections.

### Real Data
|Dataset|No. of Data Points|No. of Features|No. of Clusters|
|:---|---:|---:|---:|
|abalone|4177|8|3|
|acute-inflammation|120|6|2|
|acute-nephritis|120|6|2|
|adult|48842|14|2|
|annealing|850|31|4|
|arrhythmia|295|262|10|
|balance-scale|576|4|3|
|bank|4521|16|2|
|blood|748|4|2|
|breast-cancer-wisc-diag|569|30|2|
|breast-cancer-wisc|699|9|2|
|breast-cancer|286|9|2|
|car|1728|6|4|
|cardiotocography-10clases|2126|21|10|
|cardiotocography-3clases|2126|21|3|
|chess-krvk|28029|6|18|
|chess-krvkp|3196|36|2|
|congressional-voting|435|16|2|
|conn-bench-sonar-mines-rocks|208|60|2|
|conn-bench-vowel-deterding|990|11|11|
|connect-4|67557|42|2|
|contrac|1473|9|3|
|credit-approval|690|15|2|
|cylinder-bands|512|35|2|
|dermatology|297|34|5|
|ecoli|272|7|3|
|energy-y1|768|8|3|
|energy-y2|768|8|3|
|glass|146|9|2|
|haberman-survival|306|3|2|
|hayes-roth|129|3|2|
|heart-cleveland|219|13|2|
|heart-hungarian|294|12|2|
|heart-va|107|12|2|
|hill-valley|1212|100|2|
|horse-colic|368|25|2|
|ilpd-indian-liver|583|9|2|
|image-segmentation|2310|18|7|
|ionosphere|351|33|2|
|iris|150|4|3|
|led-display|1000|7|10|
|letter|20000|16|26|
|low-res-spect|469|100|4|
|lymphography|142|18|3|
|magic|19020|10|2|
|mammographic|961|5|2|
|molec-biol-promoter|106|57|2|
|molec-biol-splice|3190|60|3|
|monks-1|556|6|2|
|monks-2|601|6|2|
|monks-3|554|6|2|
|mushroom|8124|21|2|
|musk-1|476|166|2|
|musk-2|6598|166|2|
|nursery|12958|8|5|
|oocytes_merluccius_nucleus_4d|1022|41|2|
|oocytes_merluccius_states_2f|1022|25|3|
|oocytes_trisopterus_nucleus_2f|912|25|2|
|oocytes_trisopterus_states_5b|898|32|3|
|optical|5620|62|10|
|ozone|2536|72|2|
|page-blocks|5445|10|5|
|pendigits|10992|16|10|
|pima|768|8|2|
|planning|182|12|2|
|ringnorm|7400|20|2|
|seeds|210|7|3|
|semeion|1593|256|10|
|soybean|362|35|15|
|spambase|4601|57|2|
|spect|265|22|2|
|spectf|267|44|2|
|statlog-australian-credit|690|14|2|
|statlog-german-credit|1000|24|2|
|statlog-heart|270|13|2|
|statlog-image|2310|18|7|
|statlog-landsat|6435|36|6|
|statlog-shuttle|57977|9|5|
|statlog-vehicle|846|18|4|
|steel-plates|1941|27|7|
|synthetic-control|600|60|6|
|teaching|102|5|3|
|thyroid|7200|21|3|
|tic-tac-toe|958|9|2|
|titanic|2201|3|2|
|twonorm|7400|20|2|
|vertebral-column-2clases|310|6|2|
|vertebral-column-3clases|310|6|3|
|wall-following|5456|24|4|
|waveform-noise|5000|40|3|
|waveform|5000|21|3|
|wine-quality-red|1571|11|5|
|wine-quality-white|4873|11|6|
|wine|130|13|2|
|yeast|1350|8|5|

### Synthetic Data
|Dataset|No. of Data Points|No. of Features|No. of Clusters|
|:---|---:|---:|---:|
|aggregation|788|2|7|
|aligned_bananas|500|2|2|
|arcs|104|2|4|
|balls_and_baguettes|500|2|5|
|bars|500|2|2|
|boat|500|2|3|
|cigar|500|2|4|
|circle_2_rectangles|500|2|3|
|circle_and_3_gaussians|500|2|4|
|concentric_circles_3|500|2|3|
|enclosure|622|2|3|
|filled_circle|500|2|2|
|filled_circle_2|500|2|4|
|flower|500|2|5|
|four_corners_clear|500|2|4|
|four_corners_noise|500|2|4|
|four_lines|500|2|4|
|gaussians_1_big_2_small|500|2|3|
|gaussians_3_touching|500|2|3|
|gaussians_5_compact|500|2|5|
|gaussians_5_unequal|500|2|5|
|gestalt|399|2|6|
|half_rings|500|2|2|
|happy_wave|500|2|2|
|orange|500|2|2|
|petals|500|2|4|
|random1|500|2|4|
|random2|500|2|6|
|random3|500|2|7|
|randomised_normal|500|2|9|
|randomised_triangle|500|2|10|
|saturn|500|2|2|
|sixteen_blocks|256|2|16|
|spirals|500|2|3|
|stormclouds|500|2|2|
|t_and_u|500|2|2|
|ten_spherical|500|2|10|
|three_by_three|500|2|9|
|three_circles|500|2|3|
|two_diamonds|500|2|2|
|two_u|260|2|2|
|wingnut|500|2|2|
|worms|500|2|4|
|xor|500|2|4|
|xor_big_and_small|500|2|4|
|xor_different_cardinalities|500|2|4|
|yin_yang|515|2|4|
|atom|500|3|2|
|chainlink|500|3|2|
|hepta|500|3|7|
|tetra|500|3|4|
|torus_and_rod|500|3|2|

[^1]: Citation Soon

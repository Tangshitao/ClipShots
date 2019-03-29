# ClipShots dataset
This repository contains the ClipShots dataset introduced in our [paper](https://arxiv.org/pdf/1808.04234.pdf). The videos are [here](https://pan.baidu.com/s/1J3fdQxPUtkMe6i8moCXZ0A) or [Google cloud](https://storage.googleapis.com/clipshots/data.tar.gz). Please rename the directory ClipShots to data.tar.gz to use data.

## Introduction
ClipShots is the first large-scale dataset for shot boundary detection collected from Youtube and Weibo covering more than 20 categories, including sports, TV shows, animals, etc. In contrast to previous shot boundary detection dataset, e.g. TRECVID and RAI, which only consist of documentaries or talk shows where the frames are relatively static, we construct a database containing short videos from Youtube and Weibo. Many short videos are home-made, with more challenges, e.g. hand-held vibrations and large occlusion. The types of these videos are various, including movie spotlights, competition highlights, family videos recorded by mobile phones etc. Each video has a length of 1-20 minutes. The gradual transitions in our database include dissolve, fade in fade out, and sliding in sliding out.

## Description
The database contains 3 sets of data, training set, testing set and 'only_gradual' set. The trainig set and the 'only_gradual' set are for training and the testing set is for evaluation. For the 'only_gradual' set, we annotate the gradual transitions because of insufficent gradual transitions in training set. In `video_lists`, there are 3 files that contain the video names of them respectively. The evaluation script is in `tools`.

## Main results
We list some strong baselines here.
<table>
    <thead>
        <tr>
            <th>Methods</th>
            <th colspan=3>Cut</th>
            <th colspan=3>Gradual</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td></td>
            <td>Precision</td>
            <td>Recall</td>
            <td>F1-score</td>
            <td>Precision</td>
            <td>Recall</td>
            <td>F1-score</td>
        </tr>
        <tr>
            <td>deepSBD (Alexnet-like, origin)</td>
            <td>0.731</td>
            <td>0.921</td>
            <td>0.815</td>
            <td>0.837</td>
            <td>0.386</td>
            <td>0.528</td>
        </tr>
        <tr>
            <td>deepSBD (ResNet-18)</td>
            <td>0.765</td>
            <td>0.910</td>
            <td>0.831</td>
            <td>0.770</td>
            <td>0.622</td>
            <td>0.688</td>
        </tr>
        <tr>
            <td>DSM</td>
            <td>0.776</td>
            <td>0.934</td>
            <td>0.848</td>
            <td>0.840</td>
            <td>0.904</td>
            <td>0.870</td>
        </tr>
    </tbody>
</table>

Please refer to [this paper](https://arxiv.org/pdf/1705.03281.pdf) for deepSBD and [our paper](https://arxiv.org/pdf/1808.04234.pdf) for DSM. We also release the baseline codes [here](https://github.com/Tangshitao/ClipShots_basline). Please email shitaot@gmail.com if you have any questions.

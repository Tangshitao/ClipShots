# ClipShots dataset
This repositiory contains the ClipShots dataset introduced in our [paper](). The data is avaliable [here]()

## Introduction
ClipShots is the first large-scale dataset collected from Youtube and Weibo covering more than 20 categories, including sports, TV shows, animals, etc. In contrast to previous shot boundary detection dataset, i.e. TRECVID and RAI, which only consist of documentaries or talk shows where the frames are relatively static, we construct a database containing 4039 short videos from Youtube and Weibo. Many short videos are home-made, with more challenges, e.g. hand-held vibrations and large occlusion. The training set consists of 3539 videos, 122760 cut transitions, and 35698 gradual transitions while the evaluation set consists of 500 videos, 5876 cut transitions, and 2422 gradual transitions. The types of these videos are various, including movie spotlights, competition highlights, family videos recorded by mobile phones etc. Each video has a length of 1-20 minutes. The gradual transitions in our database include dissolve, fade in fade out, and sliding in sliding out.

## Main results
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
        
    </tbody>
</table>
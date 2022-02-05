---
layout: page
title: Defining the functional and anatomical circuitry of Parkinson's disease motor symptoms
description: Toward symptom-specific closed-loop deep brain stimulation
img: assets/img/pd_summary.png
importance: 1
category: science
---

Parkinson's disease (PD) is a complex neurodegenerative disease with heterogeneous motor phenotypes.
In order to design symptom-specific closed-loop deep brain stimulation (DBS), we simultaneously quantified several metrics of PD motor dysfunction (*e.g.* tremor, slowness) using a target-tracking task.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pd_task.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Green dot represents onscreen target, grey dot and red trace indicates subject performance. Simultaneous distance-error and tremor measurements underneath. From <a href="https://doi.org/10.3389/fneur.2020.00886">Sanderson et al, 2020</a>.
</div>

When administered in the clinic, we were able to use simple machine learning algorithms (support vector machines) to differentiate the behavior of patients with movements disorders (PD, essential tremor - ET) from age-matched controls.
In addition, we were able to characterize the unique behavioral phenotype of PD from ET.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/behavior_svm.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/pd_vs_et.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Schematic showing how metrics derived from task data differentiate between patients (green) and age-matched controls (orange) using support vector machines (MES: motor error score). Right: Plots indicate relative weights of individual behavioral metrics between patients with PD (purple) and essential tremor (ET; orange) from age-matched controls. From <a href="https://doi.org/10.3389/fneur.2020.00886">Sanderson et al, 2020</a>.

</div>

We then had patients with PD perform our task to the operating room as they underwent awake implantation of DBS electrodes.
Using microelectrode recordings from the subthalamic nucleus (STN), we were able to decode the presence of PD motor dysfunction on short-timescales (*i.e.* seconds).
Similarly to how PD has diverse phenotypes, optimal neural decoding models were patient-specific and relied on a variety of frequency bands throughout the local field potential (LFP) spectrum.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/stn_recordings.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/mes_sorted_spec.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Microelectrode recording sites within the STN across all patients with PD who performed the task intraoperatively. Right: Experimental task recording spectrograms sorted by increasing motor error score (MES). From <a href="https://doi.org/10.1088/1741-2552/abaca3">Ahn et al, 2020</a>.
</div>

Although our method of patient-specific symptom decoding was flexible to each patient's constellation of symptoms, our task also provided the opportunity to define the neurophysiologic representations of individual motor symptoms such as tremor.
By combining STN microelectrode and electrocorticography (ECoG) recordings, we were able to elucidate that tremor emerges due to tremor-frequency (3-8 Hz) oscillations in the STN, but is sustained by cortico-cortical oscillations at higher frequencies (12-20 Hz).

<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/ecog_labels.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/Diagram_v6.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: ECoG recording sites across all patients with PD who performed the task intraoperatively. Right: Synthetic model of subcortical-cortical interactions during tremor. From <a href="https://doi.org/10.1523/JNEUROSCI.0854-21.2021">Lauro et al, 2021</a>.
</div>

Future work is investigating the neural dynamics of the interplay between different motor phenotypes in PD, and applying this knowledge to inform adaptive closed-loop deep brain stimulation protocols.

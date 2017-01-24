---
title: Resting-state Functional Connectivity in Sensory and Motor Networks
	   Predicts Individual Differences in Motor Learning by Observing
author: 
- Heather R. McGregor^1,3^
- Paul L. Gribble^1,2,3^
institute: 
- ^1^ Brain and Mind Institute, Dept. Psychology, University of Western Ontario
- ^2^ Dept. Physiology & Pharmacology, Schulich School of Medicine & Dentistry, University of Western Ontario
- ^3^ Graduate Program in Neuroscience, University of Western Ontario
date: January 24, 2017
bibliography: refs.bib
csl: /Users/plg/github/styles/the-journal-of-neuroscience.csl
papersize: letter
mainfont: "Palatino"
fontsize: 11pt
linestretch: 1.5
geometry: margin=1.2in
---

# Abstract

Action observation can facilitate the acquisition of novel motor
skills, however, there is considerable inter-individual variability in
the extent to which observation promotes motor learning. Here we
tested the hypothesis that inter-individual differences in brain
function or structure can predict subsequent observation-related gains
in motor learning. Subjects underwent an anatomical MRI scan and
resting-state fMRI scans to assess pre-learning grey matter volume and
pre-learning resting-state functional connectivity (FC),
respectively. On the following day, subjects observed a video of a
tutor adapting her reaches to a novel force field. After observation,
subjects performed reaches in a force field as a behavioral assessment
of gains in motor learning resulting from observation. We found that
inter-individual differences in resting-state FC, but not grey matter
volume, predicted subsequent motor learning by observing. Pre-learning
resting-state FC among bilateral PMd, M1, S1 and left SPL was
positively correlated with behavioral measures of post-observation
motor learning. Sensory-motor resting-state FC thus predicts the
extent to which observation will promote subsequent motor learning.

\newpage

# Introduction

Recent work has shown that action observation can promote motor
learning. For example, individuals can learn how to reach in novel
robot-imposed force field (FF) environments by observing the movements
of a tutor [@Mattar:2005aa]. Subjects observed a video of a tutor
adapting his reaches to a novel robot-imposed FF applied. Subjects who
later performed reaches in the same FF as what they had observed
showed a benefit, performing better (straighter) reaches compared to
subjects who did not observe. Subjects who later performed reaches in
the opposite FF to what they had observed performed worse (more
curved) reaches than subjects who did not observe. While these results
demonstrate that FFs can be partially learned from observation, there
is considerable inter-individual variability in the extent to which
observation promotes motor learning. Little is known about why this
may be. It is feasible that some subjects are more predisposed to
learning from observation than others—whether from birth, from
experience-dependent plasticity, or a combination of these or other
individual differences. Here we test the idea that inter-individual
differences in brain function or structure can predict the extent to
which observation promotes subsequent motor learning.

In a recent review article, @Zatorre:2013aa discusses findings showing
how baseline structural and functional neural connectivity patterns
predict individual differences in musical training and speech
learning.  Other studies have shown similar predictability for a wide
array of cognitive abilities including executive function
[@Barnes:2014aa; @Reineberg:2015aa], reading [@Koyama:2011aa;
@Wang:2013aa], second language acquisition [@Chai:2016aa], visual
perceptual discrimination [@Baldassarre:2012aa] and memory recall
[@King:2015aa]. In the motor domain, recent work has examined the
neural correlates of inter-individual variability in the ability of
healthy adults to learn new motor skills through physical practice.
@Tomassini:2011aa demonstrated that inter-individual differences in
both functional and structural MRI measures correlate with the
acquisition of a novel visuomotor tracking skill. Greater task-based
functional activation in a network involving prefrontal, premotor, and
parietal cortices, as well as basal ganglia and the cerebellum was
associated with higher behavioral measures of active motor
learning. Structural differences within the premotor cortex, higher
order visual areas, and the cerebellum were also positively correlated
with learning abilities [@Tomassini:2011aa]. Similarly, using
dense-array EEG, @Wu:2014aa showed that resting-state functional
connectivity (FC) between premotor, primary motor and parietal
cortices could predict individual differences in the subsequent
learning of a visuomotor tracking task. Together, these studies
suggest that functional and structural variations in motor
learning-related brain networks can, in part, explain individual
differences in active motor learning ability. The results of these
studies raise the possibility that inter-individual differences in
brain structure or function may also predict motor learning by
observing.

Here we tested the hypothesis that inter-individual differences in
brain function or structure can predict the extent to which
individuals will learn to perform a novel sensory-motor task (FF
reaching) from observation. Based on our previous work
[@McGregor:2015aa; @McGregor:2016aa], we expected that
inter-individual differences in brain function and structure within
visual and sensory-motor brain networks would be predictive of motor
learning by observing. On day 1, subjects performed baseline (no FF)
reaches using a robotic arm and then underwent pre-learning anatomical
and resting-state fMRI scans.  Twenty-four hours later, subjects
observed a video of a tutor learning to reach in a novel FF then
performed reaches in a FF as a behavioral assessment of motor learning
by observing. We found that pre-learning (day 1) resting-state FC
among bilateral PMd, M1, S1 and left SPL predicts motor learning by
observing on day 2. In contrast, inter-individual differences in grey
matter volume could not predict subsequent motor learning by
observing. Pre-learning sensory-motor resting-state FC thus explains
part of the between-subject variation in motor learning by observing.

# Materials and Methods

## Subjects

Thirty healthy subjects participated in this study. Fifteen subjects
were assigned to a learning group (6 males, mean age 22.87 $\pm$ 1.02
(SE) years) and 15 were assigned to a control group (6 males, mean age
22.53 $\pm$ 0.86 (SE) years). All subjects were right handed, had
normal or corrected-to-normal vision, were naïve to force fields, and
reported no neurological or musculoskeletal disorders. Subjects
provided written informed consent prior to participating. All
experimental procedures were approved by the Research Ethics Board at
the University of Western Ontario.

## Apparatus

Subjects were seated in front of a custom tabletop and grasped the
handle of a two degree of freedom robotic arm (IMT2, Interactive
Motion Technologies) with the right hand (see Figure
[-@fig:robot]). The chair height was adjusted such that the subject's
upper arm was abducted approximately 90^o^ from the trunk. An air sled
was secured beneath the subject's right arm to support the arm against
gravity. A semi-silvered mirror, mounted horizontally just above the
robotic arm, occluded the subject's vision of his or her own arm and
the robotic arm. During the reaching task, an LCD monitor projected
visual feedback onto the semi-silvered mirror. Visual feedback
included a start position (20-mm blue circle), a single target (20-mm
white circle), and a cursor representing hand position (12-mm pink
circle).

The reaching task involved guiding the handle of the robotic arm from
the start position to the target, which was located 15 cm in front of
the start position. Subjects were instructed to move as straight as
possible. At the end of each reach, the target changed color to
provide feedback about movement time: the target disappeared if the
movement time was correct (450-550 ms duration), turned red if the
movement was too fast (< 450 ms) or turned green if the movement speed
was too slow (> 550 ms). Following each reach, the robotic arm
returned the subject's hand to the start position.

The robot applied a velocity-dependent force field during the reaching
task according to Equation [-@eq:forcefield]:
$$
	\begin{bmatrix} F_{x}\\  F_{y} \end{bmatrix} = 
	\begin{bmatrix} 0 &dk\\ -dk &0 \end{bmatrix}
	\begin{bmatrix} v_{x}\\  v_{y} \end{bmatrix}
$$ {#eq:forcefield}

in which $x$ and $y$ are lateral and sagittal directions, $F_{x}$ and
$F_{y}$ are the applied robot forces, $v_{x}$ and $v_{y}$ are hand
velocities, $k$=14 Ns/m, and $d$=0 (null field), +1 (right FF) or -1
(left FF).

## Reaching Video Stimuli

Each video showed a top-down view of a tutor performing the reaching
task described above using her right arm. The tutors in the videos
were naive to force fields. The learning video consisted of a series
of 30-second clips showing a tutor adapting her reaches to a leftward
force field (left FF). These clips showed the gradual progression from
curved to straight movements that is indicative of motor learning. The
control video consisted of a series of 30-second clips showing a tutor
performing reaches in an unlearnable FF in which the direction of the
FF varied randomly from trial-to-trial between a left FF, right FF, or
null field. These clips showed the tutor performing both high and low
curvature movements, but lacked the progressive decrease in movement
curvature depicted in the learning video. The videos showed 200
reaches each and were 15 minutes in duration (including regular
breaks). Video screenshots are shown in Figures [-@fig:robot]B and
[-@fig:experiment]A. Note that the dashed trajectories and
superimposed labels have been included for demonstrative purposes and
were not shown to subjects.

## Experimental Design

The experimental design is shown in Figure [-@fig:robot]B. All
subjects (n=30) participated in three sessions. For each subject, the
sessions were held at the same time on three consecutive days. On day
0, subjects were familiarized with the reaching task by performing 50
practice movements in a null field (no force applied by the robot). On
day 1, subjects performed 200 baseline reaches in the null field and
then walked to the imaging facility for a fMRI scan session (see below
for scan session details). The scan session began approximately 20
minutes following the completion of the reaching task and lasted 1
hour. Data collected during the day 1 scan session were used to
estimate pre-learning resting-state FC between a number of visual and
sensory-motor brain areas (see ROIs below) and to estimate whole-brain
grey matter volume. On day 2, subjects performed the observational
motor learning task. Subjects watched either the learning video or the
control video while seated in front of the robotic arm. The video was
played on the LCD TV positioned above the robotic arm and was
projected onto the semi-silvered mirror surface. We instructed
subjects to count the number of correctly-timed reaches in the video
(indicated by the target disappearing upon the completion of a reach)
and to report the final tally to the experimenter following the
video. Reported tallies were analyzed to verify that subjects attended
to the video, but these data were not incorporated into the behavioral
or neuroimaging analyses. Approximately 80 minutes after video
observation, we assessed motor learning by observing by having
subjects perform 100 reaches while the robotic arm applied a rightward
FF (right FF).

Note that during the 80 minutes between video observation and the
motor learning test on day 2, both groups underwent a second fMRI scan
session identical to the day 1 fMRI scan session. Data from the second
fMRI scan session were not used in any of the analyses presented here
since the main objective of the current study was predicting motor
learning by observing based on pre-learning (day 1) neuroimaging
data. See @McGregor:2015aa for details of FC changes following motor
learning by observing.

We assessed motor learning behaviorally by having subjects perform
reaches in the opposite FF to what was learned. The better subjects
learned the observed left FF, the worse their performance would be
during their initial performance in the right FF. The idea is that
during observation, subjects learn the compensatory pattern of muscle
forces (i.e., rightward compensation) that is required to counteract
the left FF. Subjects continue to use a learned pattern of muscle
forces even when the force environment is unexpectedly changed,
resulting in after-effects [e.g., @Shadmehr:1994aa]. As is the case in
this study, after-effects are especially large if the environment is
changed such that it is the opposite of the learned environment. This
is because the subject compensates rightward (persistence of the
learned pattern of muscle forces) and the robotic arm also pushes the
hand to the right. Therefore, we expected that those subjects who
better learned the observed left FF would perform highly curved
reaches when first exposed to the final right FF [@Brown:2009aa;
@Cothros:2006aa; @McGregor:2015aa; @McGregor:2016aa]. We chose to use
an interference paradigm to assess motor learning by observing because
it tends to be a more sensitive measure compared testing subjects in
the same FF that they observed.

The overall aim of this study was to assess if pre-learning
resting-state functional connectivity can predict the extent to which
subjects will learn from observation. While both the learning and
control groups underwent resting-state scans on day 1, we did not
perform neuroimaging analyses on the data from the control group. This
is because the control group did not observe learning in the control
video and so motor learning by observing could not occur. Here we have
included the control group as a basis for comparing behavior in the
final motor learning test to demonstrate the motor learning by
observing effect.

## Imaging Procedure

Neuroimaging data were acquired by a 3-T Siemens Magnetom Tim Trio
imaging system using a 32-channel head coil. All subjects underwent
resting-state scans on day 1 to assess pre-learning functional
connectivity prior to the observational motor learning task (on day
2).  The fMRI scan session lasted 1 hour. The scan session began with
two 8-minute resting-state runs during which subjects were instructed
to relax with their eyes closed. The resting-state runs were separated
by a 5-minute anatomical scan during which subjects were instructed to
fixate their gaze on a crosshair projected onto a screen. Subjects
then performed two 6-minute functional localizer tasks: an action
observation network localizer and a motor localizer task. We selected
10 *a priori* regions of interest (ROIs) known to be involved in
action observation and/or motor learning (see below). The two
localizer tasks allowed us to determine the coordinates of each ROI
for use in the functional connectivity analysis described below.

For the the action observation network localizer task, subjects viewed
intact and scrambled video clips of a tutor performing reaches while
holding the robotic arm (ten 36-s interleaved blocks). Intact video
clips showed a top-down view of a tutor performing straight reaching
movements in a null FF. For the baseline condition, subjects viewed
scrambled versions of the video clips in which only the start and
target positions remained in their original locations. Scrambling the
videos allowed us to preserve the low-level motion features such as
movement direction and velocity while removing such movement features
as shoulder and elbow joint rotations and the hand path
[@Malfait:2010aa].  During the action observation network localizer
task, subjects were instructed to count the number of correctly-timed
movements the tutor performed and to report the final tally to the
experimenter at the end of the video. This was done to verify that
subjects attended to the video. Reported tallies were not incorporated
into the behavioral or neuroimaging analyses.

For the motor localizer task, subjects performed interleaved blocks of
arm movement and rest (ten 36-s blocks). During movement blocks,
subjects slowly moved their right forearm along the frontal plane in a
cyclic manner (90^o^ elbow flexion). Color-coded visual cues were
used to pace movements at a frequency of 0.1 Hz.

## Image Acquisition

Whole-brain functional data were acquired with a T2-weighted EPI
sequence (TR = 3,000 ms, TE = 30 ms, 90^o^ flip angle, 3-mm
isotropic voxels, 80x80x50 matrix, iPAT acceleration factor =
2). T1-weighted anatomical images were collected with a MPRAGE
sequence (TR = 2,300 ms, TE = 2.98 ms, 9^o^ flip angle, 1-mm
isotropic voxels, 192x240x256 matrix).  For each subject, a field map
was acquired at the beginning of the scan session using a gradient
echo sequence (TR = 531 ms, TE = 4.92 ms/7.38 ms, 60^o^ flip
angle, 3-mm isotropic voxels, 80x80x50 matrix).

## Behavioral Data Analysis

During the reaching task, the position and velocity of the robotic
handle were sampled at 600 Hz and stored for offline analysis.
Positional data were low-pass filtered at 40 Hz. The start and end of
each trial were defined using a threshold of 5% of the peak tangential
hand velocity. Movement curvature was quantified for each trial as the
maximum perpendicular deviation of the hand (PD) from a line
connecting the start and target locations [@Mattar:2005aa].

We calculated a behavioral motor learning by observing score for each
subject. Motor learning by observing scores were calculated as the
mean PD of the first 3 reaches in the right FF minus the mean PD of
the last 50 reaches in the baseline null field. This approach allowed
us to examine the extent to which observing the left FF interfered
with learning subjects' initial performance in the right FF compared
to control subjects who did not observe the tutor undergoing
learning. As in our previous work [@Brown:2009aa; @Cothros:2006aa;
@McGregor:2016aa], we expected that motor learning by observing would
affect initial performance in the right FF, after which active motor
learning would occur for both groups to adapt to the right FF.

## Functional Connectivity Analysis

We carried out a whole-brain seed-based correlation analysis to
examine if inter-subject differences in resting-state FC could predict
the amount of motor learning by observing that subjects would achieve
on the following day. Neuroimaging data analyses were performed only
on the data from the learning group using FSL version 5.04 (FMRIB's
Software
Library,
[https://www.fmrib.ox.ac.uk/fsl](https://www.fmrib.ox.ac.uk/fsl)). Image
preprocessing steps for the functional connectivity analysis included
the removal of the first 2 volumes in each functional run,
slice-timing correction, motion correction, spatial smoothing using a
6-mm kernel, and high-pass temporal filtering (100 s). Field map
distortion correction and affine coregistration of functional and
anatomical images were performed using boundary-based registration
(BBR) in FLIRT. Subjects' images were registered to MNI space (MNI's
152-brain T1 template, 2-mm isotropic voxel size) using a 12-DOF
affine registration.

We selected 10 *a priori* regions of interest (ROIs) known to be
involved in action observation and/or motor learning. ROIs were used
in the whole-brain functional connectivity analysis described
below. These regions included left supplementary motor cortex, dorsal
premotor cortex, ventral premotor cortex, primary motor cortex,
primary somatosensory cortex, visual area V5/MT, superior parietal
lobule, inferior parietal lobule, putamen, and right cerebellum. The
coordinates of each ROI were determined based on block-design analyses
of the action observation network and motor localizer tasks described
above. For each localizer, the task-induced response was assessed with
a per-subject GLM. Data from all 15 subjects were then included in a
mixed-effects analysis (Z > 2.3, p < 0.05, cluster-based thresholding)
for each localizer. The seed coordinates were chosen as the peak
activated voxel within each of the 10 brain areas listed above. ROIs
consisted of all voxels within a 6-mm radius of the activation
peaks. Table [-@tbl:ROIs] shows the coordinates of the activation
peaks used for each ROI.

Functional connectivity analyses were performed on both resting-state
runs acquired on day 1. Following preprocessing, a bandpass filter of
0.01 – 0.1 Hz was applied to the resting-state data [@Biswal:1995aa;
@Damoiseaux:2006aa]. Mean-based intensity normalization was performed
(mean value of 10,000) to remove global intensity differences between
runs [@Damoiseaux:2006aa]. We carried out seed-based correlation
analyses on each subject's resting-state runs using FILM (FMRIB's
Improved General Linear Model). This allowed us to assess FC between
each ROI and the rest of the brain on day 1. The mean time series of
each ROI was used as the predictor of interest in the GLM.  Nuisance
regressors included the temporal derivative of the mean ROI time
series, 6 rigid body motion parameters obtained from motion
correction, mean global signal, mean white matter signal and mean CSF
signal. For each ROI, the results of the subject-level analyses were
then entered into a mixed-effects group-level analysis in which the
predictor of interest was the group mean.

Prior to the fMRI scan session on day 1, all subjects had performed
200 reaches in the null field. Even though the robot did not apply
force to the subject's hand during null field reaches, subjects likely
underwent motor learning as they learned the inertial properties
involved in moving the robotic arm. It is possible that learning
during null field reaches may have altered pre-learning FC in the
subsequent resting-state scans. To account for the potential effects
of previous experience in the null field, we included in our
group-level analysis a nuisance regressor modelling the average PD of
the last 50 reaches in the null field for each subject.

Group-level analysis results were thresholded using GRF theory-based
maximum height thresholding with a corrected significance level of
p=0.005 (voxelwise thresholding, corrected for familywise error). We
applied a Bonferroni correction for the number of ROIs used;
therefore, our corrected significance threshold of p=0.005 reflects
p=0.05/10 ROIs.  These analyses resulted in 10 Z score maps (one per
ROI) showing areas that, on average, exhibited FC with the seed region
across subjects. FC was defined as the temporal correlation (Fisher
*Z*-transformed correlation coefficient) between the seed region time
series and the average time series of all target clusters.

For each ROI, we computed the correlation between day 1 resting-state
FC and day 2 motor learning by observing scores. We again applied a
Bonferroni correction for the number of ROIs used; therefore, we
considered statistically significant only those correlations for which
p < 0.005 (i.e., p=0.05/10 ROIs).

## Voxel-Based Morphometry Analysis

We also carried out a whole-brain voxel-based morphometry (VBM)
analysis to test for inter-subject differences in grey matter volume
across the whole brain on day 1 that could predict motor learning by
observing scores on day 2. This analysis was carried out on the
T1-weighted images from the learning group using FSL-VBM v1.1. First,
each subject's anatomical image was brain-extracted, grey-matter
segmented, and transformed to MNI space using a nonlinear
registration. The resulting anatomical images were then averaged and
flipped along the x-axis to generate a left-right symmetric,
study-specific template. Grey matter images were then smoothed using a
2-mm Gaussian kernel. A voxelwise GLM modelling the subjects' motor
learning by observing scores was applied using non-parametric
permutation (50,000 iterations) to correct for multiple comparisons
with a significance threshold of p=0.005.

# Results

## Behavioral Results

Figure [-@fig:experiment]A shows the behavioral data from the learning
and control groups. It can be seen that, on day 1, reaches are
straight in the baseline null field condition for both
groups. Following video observation on day 2, we behaviorally assessed
motor learning by observing by instructing subjects to perform
straight reaches while the robotic arm applied a right (the opposite
FF to what had been observed in the learning video). The better
subjects had learned and retained the observed left FF, the worse
their performance would be during their initial performance in the
right FF. Indeed, we found that subjects who observed the tutor
adapting to a left FF in the learning video exhibited greater PD
during initial reaches in the right FF compared to control subjects
who observed the tutor performing curved reaches in an unlearnable
FF. As in previous work [@Bernardi:2013aa; @Brown:2009aa;
@Cothros:2006aa; @Mattar:2005aa; @McGregor:2016aa; @Williams:2012aa],
the effects of observation are most apparent early in the motor
learning test (i.e., the first 10 reaches shown as blocks 1 and 2 in
Fig 2A) and diminish as subjects in both the learning and control
groups adapt to the right FF. Average motor learning by observing
scores are shown in Figure [-@fig:experiment]B. Motor learning by
observing scores reflect the PD of the first 3 reaches in the right FF
relative to the subject's baseline PD in the null field. In Figure
[-@fig:experiment]B, it can be seen that those subjects who observed
the tutor undergoing left FF learning exhibited significantly higher
motor learning by observing scores compared to control subjects who
observed the tutor performing reaches in an unlearnable FF
(*t*(28)=2.58, p < 0.01).

## Functional Connectivity Analysis

We performed functional connectivity analyses on the neuroimaging data
acquired from the learning group on day 1 to examine if individual
differences in pre-learning FC could predict motor learning by
observing subjects on the following day. Of the 10 ROIs used, only the
analysis using the left S1 ROI revealed a network in which
pre-learning FC was reliably correlated with day 2 motor learning by
observing scores. As shown in Figure [-@fig:FC1], day 1 FC among left
S1 ROI and clusters in bilateral PMd, bilateral M1, bilateral S1 and
left SPL was positively correlated with day 2 motor learning by
observing scores (r=0.76, p=0.001).  Subjects with greater
pre-learning FC among these areas on day 1 went on to achieve greater
motor learning by observing on the following day.  Table
[-@tbl:clusters] shows cluster activation peaks and statistics.

Our computed motor learning by observing score took into account the
average PD of a subject's first 3 reaches in the right FF relative to
his or her baseline PD in the null field. To assess the sensitivity of
the correlation between FC and motor learning by observing scores, we
computed additional motor learning by observing scores to use in our
analysis. Additional motor learning scores reflected the average PD of
the first 4, 5, 6, 7, 8, 9 or 10 reaches in the right FF minus the
average PD of the last 50 reaches in the null field. The correlation
between day 1 FC and motor learning by observing remained significant
for all of the additional motor learning by observing scores used.

The GLM used for the group-level functional connectivity analyses
included a nuisance regressor modeling each subject's PD in the null
field during the last 50 trials. This was done to account for
potential effects of subjects having had performed null field reaches
before the resting-state scans on day 1. The clusters and correlation
with behavioral scores remained significant whether the null field
nuisance regressor reflected the average PD of the last 3, 5, 10 or 50
null field reaches or the average PD of the first 3, 5, 10 or 50 null
field reaches.

It is possible that the correlation between pre-learning FC and the
day 2 motor learning scores is a spurious correlation in the BOLD
data. To assess the validity of our result, we repeated the functional
connectivity analysis on each the resting-state runs separately. The
resting-state runs were independent, separated in time by a 5-minute
anatomical scan. Again using the ROI in left S1, we found consistent
spatial patterns of pre-learning (day 1) FC among left S1, bilateral
PMd, M1, S1 and left SPL for both individual runs (see Figure
[-@fig:FC2]).  Moreover, the correlation between pre-learning (day 1)
FC and day 2 motor learning by observing scores was statistically
significant for both resting-state run 1 (r=0.75, p=0.001) and run 2
(r=0.63, p=0.01).  Therefore, when performed on the each of the two
independent resting-state runs, our analysis yielded similar results
both in terms of the spatial extent of the clusters and the
correlations with day 2 motor learning scores. It is therefore
unlikely that our main result arises from a spurious correlation.

## Voxel-Based Morphometry Analysis

We carried out a whole-brain VBM analysis on the anatomical images
from the learning group. This was done to test if individual
differences in grey matter volume could predict subsequent motor
learning by observing scores. This analysis yielded no significant
results. We tested the sensitivity of this null result to the chosen
statistical threshold. No significant clusters were found until the p
value was raised to 0.40, at which level there was a significant
cluster in right S1. Therefore, individual differences in grey matter
volume could not account for variability in the extent to which
observation promotes motor learning.

# Discussion

Here we examined if pre-learning measures of brain function or
structure could account for individual differences in the extent to
which observation facilitates motor learning. We acquired pre-learning
measures of resting-state FC and grey matter volume using MRI prior to
an observational learning task on the following day. We found that
pre-learning (day 1) resting-state FC between bilateral PMd, bilateral
M1, bilateral S1 and left SPL was reliably correlated with behavioral
scores of motor learning by observing acquired on day 2. Those
subjects who exhibited greater resting-state FC among these
sensory-motor cortical areas on day 1 achieved greater motor learning
by observing on day 2. Individual differences in grey matter volume
could not predict subsequent motor learning by observing behavioral
scores. This finding provides further insight into the neural basis of
motor learning by observing.

The finding that pre-learning resting-state FC between PMd, M1, S1 and
SPL predicts subsequent motor learning by observing is consistent with
previous work demonstrating that M1 and the somatosensory system play
necessary roles in motor learning by observing. @Brown:2009aa used
repetitive transcranial magnetic stimulation to induce a temporary
'virtual' lesion to M1 immediately after subjects observed a FF
learning video. A subsequent behavioral assessment showed that
reducing M1 excitability following observation disrupted motor
learning by observing. These results suggest that M1 plays a key role
in motor learning by observing. We have also recently demonstrated
that the somatosensory system plays a necessary role in motor learning
by observing [@McGregor:2016aa]. We used median nerve stimulation to
occupy the somatosensory system with unrelated afferent inputs while
subjects observed a video of a tutor undergoing FF learning. During
observation, subjects received median nerve stimulation to the right
arm (the same arm used by the tutor in the video), to the left arm
(opposite the arm used by the tutor) or no stimulation. Stimulation
disrupted motor learning by observing in a limb-specific manner such
that stimulation of the right arm (observed effector) interfered with
learning, whereas stimulation applied to the opposite arm did
not. This result demonstrated that the somatosensory representation of
the observed effector is necessary and therefore must be unoccupied
during observation for motor learning by observing to occur. In a
follow-up EEG experiment, we showed that S1 cortical activity, as
assessed using somatosensory evoked potentials, increased for subjects
who observed learning by an amount that positively correlated with
subsequent behavioral motor learning by observing scores. These
results suggest that observation-induced functional changes in S1
support motor learning by observing [@McGregor:2016aa].

The network identified in the current study overlaps with the results
of recent neuroimaging studies showing that sensory-motor networks
support observational learning. Using this same dataset, we have
previously shown that observing motor learning results in changes in
resting-state FC among M1, S1, visual area V5/MT and the
cerebellum. Functional connectivity changes within this network were
related to behavioral measures of motor learning by observing,
assessed following the fMRI sessions [@McGregor:2015aa]. Moreover,
@Cross:2009aa have shown that learning new dance movement sequences
by observing recruits brain areas including premotor and parietal
cortices.  The authors reported greater activation in premotor and
parietal regions when subjects observed movement sequences on which
they had been trained (by observation) over the previous 5 days
relative to untrained movement sequences. These studies suggest that
the neural substrates of motor learning by observing includes premotor
cortex, M1, S1 and parietal cortex. This is consistent with the
results of the current study in that those subjects who exhibited
greater pre-learning resting-state FC between PMd, M1, S1 and SPL were
those who later learned the most from observation.

There are commonalities between the functional network identified in
the current study and those functional networks that have been
previously reported to predict active motor
learning. @Tomassini:2011aa showed that the task-based activation of
premotor and parietal cortices (along with prefrontal cortex, basal
ganglia and the cerebellum) is associated with higher behavioral
measures of active motor learning. @Wu:2014aa have similarly shown
that resting-state FC (as measured by high-density EEG) among M1,
premotor cortex and parietal cortex can predict active skill
acquisition. The consistency between predictive functional networks
for active and observational motor learning provides evidence in favor
of similar neural substrates for these forms of motor learning.

There is evidence from the active motor learning literature that
individual differences in brain structure can also predict motor
learning. @Tomassini:2011aa demonstrated that individual differences
in grey matter volume within the cerebellum and higher order visual
areas (V2, V3, V5/MT) can also predict behavioral measures of active
motor learning during a visuomotor tracking task. While there is
evidence for structure-based predictability of active motor learning,
in the current study we found that this was not the case for motor
learning by observing; individual differences in grey matter volume
could not account for variability in behavioral scores of motor
learning by observing.

Here we tested if pre-learning measures of brain function or structure
could predict subsequent motor learning by observing. We found that
pre-learning resting-state FC among bilateral PMd, M1, S1 and left SPL
predicted the extent to which observation would promote motor learning
on the following day. Individual differences in grey matter volume
could not predict behavioral scores of motor learning by
observing. These results demonstrate that individual differences in
resting-state FC among sensory-motor cortical brain areas can explain
part of the inter-individual variability in the extent to which
observation facilitates motor learning. This finding is consistent
with the idea that those individuals who have more 'primed'
sensory-motor circuits are more predisposed to motor learning through
observation. Pre-learning FC within the identified sensory-motor
network may be used as an indicator of the extent to which observation
will promote motor learning.  Predicting an individual's
predisposition for motor learning by observing could be valuable in a
clinical context for planning individualized rehabilitation strategies
and improving prognostic accuracy [@Stinear:2010aa].

The origin of inter-individual variability in pre-learning
sensory-motor FC is still unclear. In one scenario, it is possible
that the observed inter-individual differences in FC are a reflection
of only functional variability (not anatomical variability) within
this network. However, given the close correspondence between
anatomical and functional connectivity [e.g., @Fox:2005aa], another
scenario is that the observed differences in FC arise from
inter-individual differences in anatomical connectivity. For example,
it could be the case that greater structural connectivity between
these sensory-motor brain areas results in higher pre-learning
sensory-motor FC which, in turn, promotes greater motor learning by
observing. Since we did not acquire anatomical images other than a
T1-weighted anatomical scan, we cannot rule out the possibility that
inter-individual differences in structural connectivity among
sensory-motor brain areas predicts motor learning by observing.
Resting-state FC does not only reflect anatomical connectivity;
indeed, much work has shown that resting-state FC can be shaped by
recent experiences. Such "stimulus-rest interactions" have been
demonstrated across several domains, for example, exposure to visual
stimuli [@Lewis:2009aa] or undergoing active motor learning
[@Albert:2009aa] can induce resting-state FC. Since resting-state FC
is affected by both structure and function, it is likely the case that
both of these factors contribute to individual differences in
pre-learning sensory-motor FC.  While we cannot further pursue this
question using the current dataset, this would be an interesting
avenue for future research. Another outstanding issue is the stability
of these individual differences in pre-learning FC over time. Future
research should examine the test-retest reliability of pre-learning FC
over multiple sessions (e.g., days or weeks apart) to establish the
long-term stability of the FC patterns within the network identified
here. This would allow one to better distinguish between
within-session patterns from those more permanent structural or
functional patterns.

\newpage

# Figures

![Apparatus and Experimental Design. **A**. Subjects were seated
in front of an InMotion2 robotic arm and performed the reaching task in
a horizontal plane using the right arm. **B**. On day 1, all subjects
performed reaches in a null field (no force applied by the robot).
Subjects then underwent a pre-learning MRI scan session. The scan
session consisted of 2 resting-state runs separated by an anatomical
scan, followed by 2 functional localizer tasks. On day 2, subjects in
the learning group (n=15) observed a learning video showing a tutor
adapting her reaches to a left FF. A control group (n=15) observed a
control video showing a tutor performing curved reaches in an
unlearnable (randomly-varying) FF. Finally, all subjects performed
reaches in a right FF as a behavioral test of motor learning by
observing. FF, force field.](robot.png){#fig:robot width=6.5in}

\newpage

![Behavioral results. **A**. Experimental design showing the average
PD of reaches for each group across trial in the null field on day 1
and in the right FF on day 2. Behavioral data from the learning and
control group are shown in magenta and orange, respectively. Data are
shown as 10-trial blocks except for the first 2 blocks in the right
FF, which are shown as 5-trial blocks. Error bars represent
SEM. **B**.  Motor learning by observing scores for the learning group
(magenta) and control group (orange), reflecting PD in the right FF
relative to baseline PD in the null field. Error bars represent
SEM. FF, force field; PD, perpendicular deviation.](experiment.png){#fig:experiment width=6.5in}

\newpage

![Baseline FC predicted motor learning by observing scores.
This figure shows neuroimaging data from the learning group only.
Pre-learning (day 1) resting-state FC between the left S1 ROI (inset at
left) and clusters in bilateral PMd, bilateral M1, bilateral S1 and left
SPL. Across subjects in the learning group, the average day 1
resting-state FC within this network was positively correlated with day
2 motor learning scores. As shown in the scatterplot on the far right,
subjects who exhibited stronger resting-state FC within this network on
day 1 achieved greater motor learning by observing scores on the
following day (r=0.76, p=0.001). FC values reflect the Fisher
Z-transformed temporal correlation between the ROI time series and the
average time series of all target clusters.](FC1.png){#fig:FC1 width=6.5in}


\newpage

![Pre-learning FC from run 1 and run 2 both predict motor
learning by observing scores. This figure shows neuroimaging data from
the learning group only. Data from resting-state run 1 (shown in pink)
and run 2 (shown in blue) were analyzed separately. For both runs, the
ROI in left S1 (inset at left) exhibited resting-state FC with clusters
in bilateral PMd, bilateral M1, bilateral S1 and left SPL. For both
runs, the pre-learning (day 1) resting-state FC among bilateral PMd, M1,
S1 and left was reliably correlated with day 2 motor learning scores
across subjects in the learning group. As shown in the scatterplot on
the far right, subjects who exhibited stronger FC within the network
identified in each run on day 1 achieved greater motor learning by
observing scores on day 2. FC values reflect the Fisher Z-transformed
temporal correlation between the ROI time series and the average time
series of all target clusters within each run. FC, functional
connectivity.](FC2.png){#fig:FC2 width=6.5in}


\newpage

# Tables

| **ROI** | **MNI x** | **MNI y**  |  **MNI z** | **Z Score** |
| :------ | :-------: | :--------: | :--------: | :---------: |
| L SMA   |     -4    |    -10     |     56     |    5.93     |
| L PMd   |    -24    |    -22     |     66     |    6.02     |
| L PMv   |    -42    |     -6     |     56     |    5.16     |
| L M1    |    -26    |    -30     |     64     |    6.41     |
| L S1    |    -30    |    -36     |     62     |    6.32     |
| L V5/MT |    -42    |    -76     |      2     |    5.70     |
| L SPL   |    -22    |    -48     |     68     |    5.87     |
| L IPL   |    -60    |    -44     |     22     |    4.01     |
| L BG    |    -28    |    -14     |      8     |    4.52     |
| R CB    |     26    |    -44     |    -26     |    5.22     |

: Region of Interest (ROI) coordinates used in functional connectivity
analyses. The ROI coordinates were determined on the basis of a
block-design analyses of the action observation network and motor
localizer tasks. The seed coordinates were chosen as the peak
activated voxel within each of the 10 *a priori* selected brain
regions listed in this table. L, left; R, right; SMA, supplementary
motor area; PMd, dorsal premotor cortex; PMv, ventral premotor cortex;
M1, primary motor cortex; S1, primary somatosensory cortex; V5/MT,
middle temporal visual area; SPL, superior parietal lobule; IPL,
inferior parietal lobule; BG, putamen; CB, cerebellum. {#tbl:ROIs}


\newpage

| **x** | **y** |
| ----- | ----- |
|   1   |   2   |

: Clusters in which pre-learning resting-state FC (on day 1) predicted
day 2 motor learning by observing scores. Z score activation peaks,
coordinates and anatomical labels of the sensory-motor clusters in the
identified functional network. ROI, region of interest; L, left; R,
right; SMA, supplementary motor area; PMd, dorsal premotor cortex; M1,
primary motor cortex; S1, primary somatosensory cortex; SPL, superior
parietal lobule; FC, functional connectivity. {#tbl:clusters}

\newpage
\singlespace

# References


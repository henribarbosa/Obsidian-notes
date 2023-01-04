 2022-09-12  12:29

Status: [[idea]] 

Tags: [[toInvestigate]]

# IDEAS
* How does the bidispersed bed circulates? {1} 
	* With or without mixing? {2}
	* Is there a critical angle or velocity that changes de behaviour? [[Obliquity]]
	* Direction of "vorticity" of the particles
	* Does it have a change of behaviour with velocity (channeling) {3}

# To-do
* Pre-processing images
	* Ask Danilo what he does
	* Make a new program to perform this ✅
		* --method=build_mask ✅
		* --method=apply_mask ✅
	* Subtract background ✅
	* Homogenize the picture (adjust bright and dark for each area)? Remove shadows? 
	* Try to make then binary keeping the ratio beetwen bright and dark constant inside plugs?
* Processing images
	* Find column width automatically (for the first frame only) ✅
	* Mark bottom and plugs (bottom for the first frame only) (plugs trough estimated solid fraction?)
	* Mark layer separation (and maybe the size of the mixture layer)
	* Display particle label (different color for the first apearence)
	* Calculate velocity fields ( $x$, $y$, $v_x$, $v_y$)
	* Save particles trajectories ($t_{ini}$ , $N_{frames}$ , \\n ($x$, $y$,)) in a file when the particle is lost
* Processing simulations
	* Compute bed expansion
	* Compute average granular temperature
	* Compute number os plugs (maybe through solid fraction?)
* Post-processing
	* Imput images scale here (easier to fix) and all other relevant scales
	* Read files from previous steps
	* New Python program to compare expansion over time (line graph) --method=expansion
	* Compare average granular temperature (line graph) --method=temperature
	* Compare number of plugs (line graph) --method=plugs
	* --method=all
* Computing
	* Parallelize hungarian method



b1 + w1 / b2 + w2
b1 + w2 = w2 + (t - w1 -b2 - w2) = t - w1 - b2
w1 - w2

---
# References
{1} [[@ChaikittisilpAnalysisOfSolidParticleMixing]]
{2} [[@JMValverdeEffectOfInclinationOnGasFluidized]]
{3} [[@DPODeaTheEffectOfInclination]]

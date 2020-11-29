# monitor
Estimates fault parameters based on the available centroid moment tensor determinations

# Monitors Centroid Moment Tensors from various agencies and calculates theoretical fault planes for calculation of ground deformation
# Pierre Briole 8 December 2017 - v1.0 - 29 November 2019 - v2.0 - 3 December 2019 v3.1 - 29 November 2020 v 3.2
#
# The program can be used manually or inserted in a cron table
# The output is formatted for input in the inverse6 code, see https://doi.org/10.5281/zenodo.1098391
#
# The definition of the fault size and slip is adapted from the following papers:
# Thingbaijam, K.K.S., Martin Mai, P. & Goda, K., 2017. New Empirical Earthquake Source-Scaling Laws, BSSA, 107(5), 2225–2246, http://doi.org/10.1785/0120170017
# Wells, D.L. & Coppersmith, K.J., 1994. New empirical relationships among magnitude, rupture length, rupture width, rupture area, and surface displacement, BSSA, 84(4), 974-1002.
# The rigidity of the crust is assumed to be u = 3 10^10 Pa
# If sd = surface of the fault x slip, then sd = M/u where M is the seismic moment (published by the seismological centres)
# The length is assumed to be ll = (sd * 15000 ) ^ 1/3
# The width is assumed to be wi = ll/1.6
# Those approximations are sufficient to provide first order parameters of the faults good enough to predict the displacements at the GPS stations located around the fault
# When GPS data are available, the fault paramters can be ajusted using a elastic model (e.g. Okada Y., 1992. Internal deformation due to shear and tensile faults in a half space, BSSA, 82, 1018–1040.
# And an inverse programme (e.g. inverse6, https://doi.org/10.5281/zenodo.1098391)


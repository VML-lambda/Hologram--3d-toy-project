# Time-multiplexed neural holography optical setting
- project paper: https://www.computationalimaging.org/publications/time-multiplexed-neural-holography/


1. Setting
prop_dists_rgb  = [[7.76*cm, 7.96*cm, 8.13*cm, 8.31*cm, 8.48*cm, 8.72*cm, 9.04*cm],
                   [7.77*cm, 7.97*cm, 8.13*cm, 8.31*cm, 8.48*cm, 8.72*cm, 9.04*cm],
                   [7.76*cm, 7.96*cm, 8.13*cm, 8.31*cm, 8.48*cm, 8.72*cm, 9.04*cm]]

training_plane_idxs = [0, 1, 2, 3, 5, 6]
heldout_plane_idxs = [4]
mid_idx = [3]

wavelength      = [636.4 * nm, 517.7 * nm, 440.8 * nm]
feature_size    = (10.8 * um, 10.8 * um)
image_res = (800, 1280)
slm_res   = (800, 1280)
roi_res   = (700, 1190)
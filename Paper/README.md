# Time-multiplexed neural holography optical setting
- project paper: https://www.computationalimaging.org/publications/time-multiplexed-neural-holography/


## Setting
- optical setting
    - eyepiece      = 0.12*cm (eyepiece focal length)
    - prop dist 
        - red       = [7.76*cm, 7.96*cm, 8.13*cm, 8.31*cm, 8.48*cm, 8.72*cm, 9.04*cm] 
        - green     = [7.77*cm, 7.97*cm, 8.13*cm, 8.31*cm, 8.48*cm, 8.72*cm, 9.04*cm]
        - blue      = [7.76*cm, 7.96*cm, 8.13*cm, 8.31*cm, 8.48*cm, 8.72*cm, 9.04*cm]
    - wavelength    = [636.4*nm, 517.7*nm, 440.8*nm]
    - feature_size  = (10.8*um, 10.8*um)
    - resolution
        - image_res = (800, 1280)
        - slm_res   = (800, 1280)
        - roi_res   = (700, 1190)

- Green
prop_dist       = 8.31*cm
prop_dist_green = 7.97*cm
wavelength      = 517.7*nm
prop_dists_from_wrp   = [p - 8.31*cm for p in [7.77*cm, 7.97*cm, 8.13*cm, 8.31*cm, 8.48*cm, 8.72*cm, 9.04*cm]]
                      = [-0.54*cm, -0.34*cm, -0.18*cm, 0*cm, 0.17*cm, 0.41*cm, 0.73*cm]
physical_depth_planes = [-0.54*cm, -0.34*cm, -0.18*cm, 0*cm, 0.17*cm, 0.41*cm, 0.73*cm]
virtual_depth_planes  = [1 / (physical_depth_planes[0] + eyepiece - p) - 1 / eyepiece for p in physical_depth_planes] (?)

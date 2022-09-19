# image3Dviewer

This is a module to view a 3D matrix, or a list of 2D matrix (2D numpy array). 
It used the library pyqtgraph and spinmob.egg to plot in 2D the 2D matrix for each slices. 

I created this before that I notice the existence of nice 3D viewer, as ITK-Snap for MRI, which uses nifty files. 
A nifty file can be simply created from a 3D matrix:

import nibabel as nib
new_image = nib.Nifti1Image(my3DMatrix, 
                            affine=np.eye(4))
nib.save(new_image, 'my_file.nii')

But the present module as nothing to do with nifty file. 


A simple way to show the list of 2D matrix (or to show the 3D matrix) is like this, with "images.py"
self = GUIimage()
self.show()
self.set_list_image(list_image)
Where list_image is a list of 2D numpy array (Or a 3D matrix). 

More information will come up !

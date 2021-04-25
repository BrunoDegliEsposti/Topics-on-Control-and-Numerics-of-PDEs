


----------------------- Decomposition of the domain ------------------------------

decompunif.edp: create the uniform partition of the subdomain
decompMetis.edp: use Metis to create the decomposition

----------------------- Partition of unity ------------------------------

createPartition.edp: an auxiliary file that contains the routines
"AddLayers" et "SubdomainsPartitionUnity"

------------------------------ Two-level RAS using deflation---------------------

schwarz-laplace-coarse.edp: Two-level RAS in a BiCGstab using deflation

This file includes six other files:

"createPartition.edp";

"decompunif.edp";

"globaldata.edp"; defines the global variational problem and the global matrix-vector product  

"localdata.edp"; creates the partition of unity and local problem matrices.

"buildBNN.edp"; builds the coarse preconditioned

"BiCGStab-solve-CS.edp"; Two-level RAS-preconditioned BiCGstab solver.


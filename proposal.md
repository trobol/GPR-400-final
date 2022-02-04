Thornton Fernbacher & Aidan Murphy
GPR-400
2/4/2022
 
# Project Proposal
 
 
Traditional mesh rasterization methods represent high level detail using images. This presents a challenge as increases in quality require an exponential amount of memory in comparison. Triangle based meshes also present challenges for ray tracing as they lack inherent spatial partitioning. In the face of these challenges there has been a search for alternative ways of representing 3d space. One that has increasing popularity is volumetric pixels or voxels. As voxels store the volume of the world on a very granular level they can offer more speed and features than traditional meshes in the right context. Voxels however struggle to compete in the area of animation. In this paper we seek to create a method of storing, animating and rendering volumes that move towards solving that issue.
    
Before we decided on this topic we also explored liquid simulations in a voxel environment and a specialized shader profiling tool. We decided against liquid simulations because the area is already highly saturated and it did not interest us as much as voxel animation. The profiling tool presented substantial risks as we did not know if we could get the low level access that would be required to do the things we wanted.
 
There are several methods of storing and rendering volumetric data with various advantages and disadvantages. These methods are usually based around optimizing memory space, rendering time or rendering fidelity. We seek instead to design a volumetric representation and method for rendering it that lends itself to animation.
This representation should be able to express similar movements as a mesh based animation and will be novel or a meaningful innovation on an existing representation.
 
As we are trying to create a voxel representation that is useful using current tools and hardware, all that is necessary is a CPU and GPU that are near modern and use a similar architecture. 
 
By exploring an emerging field in rendering we are helping to push the boundaries of rendering and demonstrating our interest in innovation.
 
 
## Annotated references:

Domaradzki, Jakub, and Tomasz Martyn. “Fracturing Sparse-Voxel-Octree Objects Using Dynamical Voronoi Patterns.” DSpace at University of West Bohemia: NO TITLE, Václav Skala - UNION Agency, 1 Jan. 1970, https://otik.uk.zcu.cz/handle/11025/29529.
In this article they use Voronoi-based methods in order to fracture objects that are being represented by sparse voxel octrees. They use the fractured pieces, which are able to be created efficiently and robustly, to treat each one as a simulated rigid body. After talking about that they then move onto talking about collision detection using these methods. 

Laine, Samuli. Efﬁcient Sparse Voxel Octrees - NVIDIA. https://www.nvidia.com/docs/IO/88889/laine2010i3d_paper.pdf.
This paper looks to explore the possibilities of using voxel representations as a way to display complex shapes. They go in detail about how to use voxel data structures, like sparse octrees in order to be efficient. They talk about how to build one and make it take up as little memory as possible while still being extremely useful.

Leuven, Jeroen Baert KU, et al. “Out-of-Core Construction of Sparse Voxel Octrees.” Out-of-Core Construction of Sparse Voxel Octrees | Proceedings of the 5th High-Performance Graphics Conference, 1 July 2013, https://dl.acm.org/doi/abs/10.1145/2492045.2492048
This article focuses on how to build a sparse voxel octree. It talks about how there are not many scenes that are available in this form. They give examples on how to build an out of core build algorithm that can handle the meshes.

Liu, Lingjie, et al. “Neural Sparse Voxel Fields.” Advances in Neural Information Processing Systems, 1 Jan. 1970, https://proceedings.neurips.cc/paper/2020/hash/b4b758962f17808746e9bb832a6fa4b8-Abstract.html
This is an alternative to using sparse voxel octrees. This instead talks about using neural sparse voxel fields. Which is a neural scene representation for fast and high-quality rendering. It uses raymatching techniques in order to understand the underlying voxel structure. This method is 10 times faster. 

Espe, Asbjørn Engmark, et al. Efficient Animation of Sparse Voxel Octrees for Real-Time Ray Tracing. 2019.
https://arxiv.org/abs/1911.06001
This method splits the octrees into separate parts that can be animated by manipulating their transform. It also contains a method for ray tracing non axis aligned voxels. Its limitations are that it can not bend or manipulate the shapes, limiting its utility for non rigid animations. 


















 
 
## Notes: 
(included in case that is clearer or preferable)
 
 
Proposal: Write a brief proposal for your project.  You are effectively pitching what you would like to do and why it is a good use of your time.  Include at minimum the following information: 
What is the topic you are most interested in exploring and why does it interest you?
Voxel animation method, voxel representation method
What are some other topics you have considered and what are the pros and cons compared to that selected?
Liquid Simulation in a voxel engine
Exploring shader compilation efficiency and how what is causing your shaders to run slow
What is the main point of innovation for your preferred topic?
Existing solutions often begin with a method of representing volume and seek a way to animate it. We are trying that process in reverse.
What is the research value of your topic?
Animation remains an area that limits widespread use of volume based rendering
What are your tangible goals and objectives for the final project?
A method of representing volume that is efficiently and expressly animatable, either entirely novel or a meaningful innovation on an existing format 
Animatable voxel characters
What are your hardware and software needs for achieving your objectives?
Semi-modern graphics processor and cpu
Voxel engine and 	
What steps do you foresee needing to take to achieve your objectives?
Examine in detail existing methods and the limitations of those areas. 
Why is this relevant to the industry at-large and how will it advance the field?
Makes voxels more viable for games
Why is this relevant to your professional development and how will it advance your career?
Emerging field of research


	



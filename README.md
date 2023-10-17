因修改文件眾多，且整體容量龐大，所以僅做記錄。
# Vulkan-GLTF-BSSRDF-Practice
以[vk_raytracing_tutorial_KHR](https://github.com/nvpro-samples/vk_raytracing_tutorial_KHR)為基底，
和修改其中的ray_tracing_gltf來實作次表面散射。
因計算最正確的BSSDRF較為複雜且緩慢，所以採用近似值的算法。
使用的模型為[Normalized Diffusion](https://graphics.pixar.com/library/ApproxBSSRDF/)，
雖然此為經驗所得出的模型，但是卻能高度近似於真正的BSSRDF，且計算量減少許多。
BSSRDF Importance Sampling則採用[此方法](https://gao-duan.github.io/blogs/bssrdf/index.html)
# Result
![image](https://github.com/zz4634266/Vulkan-GLTF-BSSRDF-Practice/blob/main/result.png)

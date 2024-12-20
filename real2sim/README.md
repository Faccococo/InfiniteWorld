# Real2Sim: Depth-Regulaized PGSR Reconstruction

Ref: 

[PGSR: Planar-based Gaussian Splatting Reconstruction](https://github.com/zju3dv/PGSR)

[3D Gaussian Splatting for Real-Time Radiance Field Rendering](https://github.com/graphdeco-inria/gaussian-splatting/tree/dev?tab=readme-ov-file#depth-regularization)

[Depth Pro: Sharp Monocular Metric Depth in Less Than a Second](https://github.com/apple/ml-depth-pro)  

## Depth-Regulaized PGSR Reconstruction

<!DOCTYPE html>
<html lang="en">

<body>
    <h2>Reconstruction Performance Comparison</h2>
    <table>
        <tr>
            <th></th>
            <th>GauStudio</th>
            <th>SuGaR</th>
            <th>PGSR</th>
            <th>Ours</th>
            <th>GT</th>
        </tr>
        <tr>
            <td>Screen</td>
            <td><img src="img/render_result/gs/0112.png" alt="Screen GS"></td>
            <td><img src="img/render_result/sugar/0112.png" alt="Screen SuGaR"></td>
            <td><img src="img/render_result/pgsr/0112.png" alt="Screen PGSR"></td>
            <td><img src="img/render_result/pgsr_dn/0112.png" alt="Screen Ours"></td>
            <td><img src="img/render_result/gt/0112.png" alt="Screen GT"></td>
        </tr>
        <tr>
            <td>Door</td>
            <td><img src="img/render_result/gs/0016.png" alt="Door GS"></td>
            <td><img src="img/render_result/sugar/0016.png" alt="Door SuGaR"></td>
            <td><img src="img/render_result/pgsr/0016.png" alt="Door PGSR"></td>
            <td><img src="img/render_result/pgsr_dn/0016.png" alt="Door Ours"></td>
            <td><img src="img/render_result/gt/0016.png" alt="Door GT"></td>
        </tr>
        <tr>
            <td>Wall</td>
            <td><img src="img/render_result/gs/0019.png" alt="Wall GS"></td>
            <td><img src="img/render_result/sugar/0019.png" alt="Wall SuGaR"></td>
            <td><img src="img/render_result/pgsr/0019.png" alt="Wall PGSR"></td>
            <td><img src="img/render_result/pgsr_dn/0019.png" alt="Wall Ours"></td>
            <td><img src="img/render_result/gt/0019.png" alt="Wall GT"></td>
        </tr>
        <tr>
            <td>Cabinet</td>
            <td><img src="img/render_result/gs/0073.png" alt="Cabinet GS"></td>
            <td><img src="img/render_result/sugar/0073.png" alt="Cabinet SuGaR"></td>
            <td><img src="img/render_result/pgsr/0073.png" alt="Cabinet PGSR"></td>
            <td><img src="img/render_result/pgsr_dn/0073.png" alt="Cabinet Ours"></td>
            <td><img src="img/render_result/gt/0073.png" alt="Cabinet GT"></td>
        </tr>
        <tr>
            <td>Desk</td>
            <td><img src="img/render_result/gs/0024.png" alt="Desk GS"></td>
            <td><img src="img/render_result/sugar/0024.png" alt="Desk SuGaR"></td>
            <td><img src="img/render_result/pgsr/0024.png" alt="Desk PGSR"></td>
            <td><img src="img/render_result/pgsr_dn/0024.png" alt="Desk Ours"></td>
            <td><img src="img/render_result/gt/0024.png" alt="Desk GT"></td>
        </tr>
    </table>
    <p><strong>Figure 1:</strong> The reconstruction performance of GauStudio, SuGaR, PGSR, and our proposed method on real-world captured images is evaluated. Compared to 3DGS and SuGaR, PGSR provides an improved visual experience. Building upon PGSR, our method incorporates regularization loss terms for depth and normal vectors, achieving smoother planar surfaces, such as walls, doors, and screens, and demonstrating more robust handling of transparent surfaces like glass.</p>
</body>
</html>


## Usage

Please refers to README at [post-process](https://github.com/pzhren/InfiniteWorld/blob/master/real2sim/post-process/README.md) and [depth-real2sim](https://github.com/Faccococo/PGSR?tab=readme-ov-file#pgsr-planar-based-gaussian-splatting-for-efficient-and-high-fidelity-surface-reconstruction)
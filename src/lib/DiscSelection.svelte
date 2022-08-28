<script lang="ts">
  import {
    Canvas,
    Mesh,
    PerspectiveCamera,
    AmbientLight,
    DirectionalLight,
  } from "svelte-cubed";
  import { BoxGeometry, MeshStandardMaterial, Color } from "three";
</script>

<Canvas background={new Color("gray")}>
  <Mesh
    geometry={new BoxGeometry()}
    material={new MeshStandardMaterial({ color: 0xff3e00 })}
    scale={[1, 1, 1]}
    rotation={[0, 0, 0]}
  />
  <PerspectiveCamera position={[1, 1, 3]} />
  <AmbientLight intensity={0.6} />
  <DirectionalLight intensity={0.6} position={[-2, 3, 2]} />
</Canvas>

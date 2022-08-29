<script lang="ts">
  import { Canvas, Mesh, PerspectiveCamera, AmbientLight, DirectionalLight } from "@threlte/core";
  import { Text } from "@threlte/extras";
  import { BoxBufferGeometry, MeshStandardMaterial, Color } from "three";
  const DEG = Math.PI / 180;
</script>

<Canvas>
  <Mesh
    geometry={new BoxBufferGeometry(1, 1, .1)}
    material={new MeshStandardMaterial({ color: 0xff3e00 })}
    rotation={{ y: 45 * DEG }}
  />
  <PerspectiveCamera position={{ x: 1, y: 0, z: 3 }} />
  <AmbientLight intensity={0.6} />
  <DirectionalLight intensity={0.6} position={{ x: -2, y: 3, z: 2 }} />
</Canvas>

## English
[Download](https://github.com/lilxyzw/lilTextureUtil/releases)

1. Drag and drop unitypackage to the Unity window to import it.
2. Right-click on the texture and select `_lil/TextureUtil/*` to convert

Since the G and B channels are set to 1.0 when converting to `MetallicGlossMap`, in many cases it can be used as a `Mask Map` as is. Basically, convert with `Perceptual Roughness`, and if the result is too smooth, convert with `Roughness`.

## 日本語
[ダウンロード](https://github.com/lilxyzw/lilTextureUtil/releases)

1. unitypackageをUnityウィンドウにドラッグ＆ドロップでインポート
2. テクスチャを右クリックして`_lil/TextureUtil/`内のメニューから変換

`MetallicGlossMap`変換時にG・Bのチャンネルに1.0が設定されるため、多くの場合はそのまま`Mask Map`として使用できます。基本的に`Perceptual Roughness`として変換を行い、結果が滑らかすぎる場合は`Roughness`で変換を行ってください。

## Selection and conversion

|Menu Name|Selection (Bold is required, others are optional)|Output|
|-|-|-|
|[Texture] Convert normal map (DirectX <-> OpenGL)|**Normal map**|Normal map|
|[Texture] Smoothness/Smoothness -> MetallicGlossMap|**Smoothness**|MetallicGlossMap|
|[Texture] Smoothness/Metallic, Smoothness (, Occlusion, Detail) -> MetallicGlossMap (MaskMap)|**Metallic**, **Smoothness**, Occlusion, Detail|MetallicGlossMap or Mask Map|
|[Texture] Perceptual Roughness/Roughness -> Smoothness|**Roughness**|Smoothness|
|[Texture] Perceptual Roughness/Roughness -> MetallicGlossMap|**Roughness**|MetallicGlossMap|
|[Texture] Perceptual Roughness/Metallic, Roughness (, Occlusion, Detail) -> MetallicGlossMap (MaskMap)|**Metallic**, **Roughness**, Occlusion, Detail|MetallicGlossMap or Mask Map|
|[Texture] Roughness/Roughness -> Smoothness|**Roughness**|Smoothness|
|[Texture] Roughness/Roughness -> MetallicGlossMap|**Roughness**|MetallicGlossMap|
|[Texture] Roughness/Metallic, Roughness (, Occlusion, Detail) -> MetallicGlossMap (MaskMap)|**Metallic**, **Roughness**, Occlusion, Detail|MetallicGlossMap or Mask Map|
---
layout: default
title: "Unity Editor Only"
tags: tips blog
image: /assets/img/file.ico
---

## Keeping Unity scripts and objects out of builds
Something that I find becomes necessary the more I work on projects in Unity, is keeping certain objects and scripts in the editor and out of builds. I usually keep around objects for notes and todo-lists in scenes, as well specific file loaders/unit testers. Needless to say, trying to keep track of every object in scenes and deleting and recreating them before and after builds would be a headache. At first I had tried putting scripts in an Editor folder to keep them out of builds, but of course Unity doesn't allow Editor scripts to reside on GameObjects. There were actually two steps to keeping certain scripts and objects out of builds with ease.

The first step may seem like a bit of common sense, but wrapping an entire script in a pre-processor directive would allow it to only exist in the editor, like the class below.
```cs
#if UNITY_EDITOR
using UnityEngine;

public class EditorNotes : MonoBehaviour
{
    [TextArea(15, 1000)] public string notes;
}
#endif
```

So that keeps certain scripts out of builds, but what about the objects they're attached to? As it is, a lot of "Missing MonoBehaviour" warnings will appear in the game's output log. This took a bit of searching to come across, and I had missed it initially since I had gotten away from tagging objects. Unity comes with a few tags for GameObjects out of the box, but one is called "EditorOnly" and tells Unity to not include that object when building. A handy feature for keeping back test objects across an entire projects instantly.
![EditorOnly tag](/images/unity-tips/editor-only.png)

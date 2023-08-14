# just_audio
Audio Player

fork 目的：
在单曲循环下，无法进行上一首/下一首
注释
```
int? _getRelativeIndex(int offset) {
    if (_audioSource == null || currentIndex == null) return null;
    // 注释此行，单曲循环的判断
    // if (loopMode == LoopMode.one) return currentIndex;
    final effectiveIndices = this.effectiveIndices;
    // 省略...
}
```

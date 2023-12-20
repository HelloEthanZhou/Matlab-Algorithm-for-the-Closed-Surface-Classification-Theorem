# 闭曲面分类定理的Matlab算法

这个仓库包含了一个用于计算闭曲面分类定理的Matlab算法。该算法可以计算闭曲面的顶点类数和顶点类矩阵，并给出闭曲面的类型、边数以及节点类数。

## 函数说明

`nodeClass`：计算闭曲面的顶点类数和顶点类矩阵。

`stringToMatrix`：将输入字符串转换为矩阵表示。

`closedSurfaceType`：计算闭曲面的类型、边数和节点类数。

## 使用方法

1. **准备工作**

   在Matlab环境中运行算法前，确保已经准备好相关的输入字符串。输入字符串的格式应为一个字母+其他类型(或没有)+一个字母+其他类型(或没有)+...，其中相同字母仅输入两次。例如：`ab^-1a0cdcbd`。

2. **运行算法**

   在Matlab中调用 `closedSurfaceType` 函数，传入准备好的输入字符串。该函数将返回闭曲面的类型、边数和节点类数。

   ```matlab
   % 例如
   string = 'ab^-1a0cdcbd';
   [type, edgeNumber, nodeNumber] = closedSurfaceType(string);
   ```

3. **查看结果**

   算法运行完成后，你可以通过输出结果来获取有关闭曲面的信息。

   ```matlab
   fprintf('边数为:%d\n', edgeNumber)
   fprintf('节点类数为:%d\n', nodeNumber)
   fprintf('闭曲面类型为:%s\n', type)
   ```

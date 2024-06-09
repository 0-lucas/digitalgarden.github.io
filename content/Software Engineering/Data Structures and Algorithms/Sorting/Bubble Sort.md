# What is it?

*Bubble sort* is one of the simplest [[Sorting Algorithms]], based in **repeatedly swapping neighbor elements** if they are in the wrong order.

For **each data point**, it iterates through the whole [[Array]]. This creates an $O(n^2)$ complexity, **running through every single data point twice**, in a worst-case scenario, making it **very slow for large datasets**.

One of the benefits of *bubble sorting* is that because everything is made *in place*, **no additional available memory is required**. This is important for memory-restricted devices.

```csharp
public class BubbleSort: ISortAlgorithm
{
    // Passes one time through entire array, swapping any corresponding elements.
    private static List<int> SortUnitIteration(List<int> Data)
    {
        for (int i = 0; i < Data.Count - 1; i++)
        {
            if (Data[i] > Data[i + 1])
            {
                Data = HelperMethods.Swap(Data, i, i + 1);
            }
        }

        return Data;
    }

    // Applies one sorting iteration for each data point.
    public List<int> Sort(List<int> Data)
    {
        for (int n = 0; n < Data.Count; n++)
        {
            List<int> Data = SortUnitIteration(Data);
        }
        
        return Data;
    }
}
```
---
-api-id: P:Windows.AI.MachineLearning.Preview.InferencingOptionsPreview.PreferredDeviceKind
-api-type: winrt property
---

<!-- Property syntax.
public LearningModelDeviceKindPreview PreferredDeviceKind { get;  set; }
-->

# Windows.AI.MachineLearning.Preview.InferencingOptionsPreview.PreferredDeviceKind

## -description
Gets or sets the preferred device that the evaluation will be performed on.

## -property-value
The preferred device. The default value is LearningDeviceAny.

## -remarks

## -see-also

## -examples
public void SetEvaluationOptionsForModel(LearningModelPreview model)
{
    // Set our preference to use the GPU
    InferencingOptionsPreview options = model.InferencingOptions;
    options.PreferredDeviceKind = LearningModelDeviceKindPreview.LearningDeviceGpu;
 
    model.InferencingOptions = options;
}
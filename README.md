# IAC_PIPELINE_1.8
IaC Pipeline 1.8
- This release works with two GitHub Repos
  + IaC - Single Component
  + Pipeline Buildspecs
- Include parameters:
  + TemplateFileName
  + ParameterFileName
  + StackName
- CloudFormation Operation: create-change-set
  + Allows CF Template from:
    - Local File (Max.  51,200 bytes)
    - S3 Bucket  (Max. 460,800 bytes)
  + Allows CF Nested Templates from:
    - S3 Bucket
  + Does not allow parameters from an S3 Bucket
  + Only allows parameters from:
    - CLI Key=Value pairs
    - Local JSON file
- S3 Buckets
  + CodePipeline Artifact bucket automatically created
  + IaC bucket optionally created

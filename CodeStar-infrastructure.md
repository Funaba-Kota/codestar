# Resourceの種類  

|リソース名|サービス|用途|詳細|
|-|-|-|-|
|HelloWorld|Lambda||FunctionName(処理名)：awscodestar-"パラメータ設定値"-lambda-HelloWorld<br>Handler(実行を呼び出すための関数)：index.handler<br>Runtime：nodejs16.x<br>Environment(ランタイム環境):環境変数NODE_ENVをproductionに設定<br>Role(権限): IAMロールLambdaExecutionRoleのARNを設定<br>Events(イベント定義):GET/POSTリクエストに応答<br>CodeUri(コードが格納されているS3バケットのURI)s3://aws-codestar-ap-northeast-1-941920968752-funaba0601-back-pipe/676c11011300f6808b2da5cbc44c6c2d|
|LambdaExecutionRole|IAM Role||RoleName(ロール名)：CodeStar-"パラメータ設定値(ProjectTd)"-Execution"パラメータ設定値(Stage)"<br>AssumeRolePolicyDocument(信頼ポリシー)：LambdaがこのIAMロールを引き受けることを許可<br>Path(リソースのパス)：ルート<br>ManagedPolicyArns(ロールにアタッチするARN)：AWSLambdaBasicExecutionRoleを設定<br>PermissionsBoundary(権限境界)：CodeStar_"パラメータ設定値(ProjectTd)"_PermissionsBoundaryのポリシーを設定｜


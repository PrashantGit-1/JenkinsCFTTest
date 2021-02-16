pipeline {
	agent any
	stages {
		stage( 'clone repo' ) {
			steps {
			sh "export AWS_DEFAULT_REGION=ap-south-1a"
			sh "aws cloudformation create-stack --stack-name myteststack --template-body file://s3bucket.json --region 'ap-south-1a'"
			}
		}
	}
}	
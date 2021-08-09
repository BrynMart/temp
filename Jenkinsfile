node {
	stage 'Checkout'
		checkout scm

	stage 'Build'
		make

	stage 'Archive'
		archive 'ProjectName/bin/Release/**'

}

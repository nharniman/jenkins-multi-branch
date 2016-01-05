node {
    echo "Branch Name: ${env.BRANCH_NAME}"
    
    if (env.BRANCH_NAME =~ /developer*/) {
	    echo "Matched Developer"
        flow = load 'developer.groovy'
    } else if (env.BRANCH_NAME =~ /release*/) {
	    echo  "Matched Release"
        flow = load 'release.groovy'
    } else {
    
    echo "Not Matched"
    }
}

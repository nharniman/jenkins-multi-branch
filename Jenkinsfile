node {
    echo "Branch Name: ${env.BRANCH_NAME}"
    
    if (BRANCH_NAME =~ /developer*/) {
	    echo "Matched Developer"
        flow = load 'developer.groovy'
    } else if (BRANCH_NAME =~ /release*/) {
	    echo  "Matched Release"
        flow = load 'release.groovy'
    } else {
    
    echo "Not Matched"
    }
}

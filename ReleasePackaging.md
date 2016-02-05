## Release Packaging Steps ##

  * Tag the release: `svn copy -m "Tagging x.y.z release" https://ajaxslt.googlecode.com/svn/{trunk,tags/release-x-y-z}`
  * Copy the tag to a labeled directory: `cp -r release-x-y-z ajaxslt-x.y.z`
  * Create the code package: `tar cvfz ajaxslt-x.y.z.tar.gz ajaxslt-x.y.z/{AUTHORS,COPYING,ChangeLog,Makefile,README,TODO,test/{*js,*html},*js,*html}`
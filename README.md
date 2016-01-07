# debcya

Take note of package status before an upgrade and help with downgrading if
something went wrong.

## Usage

Before an upgrade, take note of the system status:

    debcya --save=`date +%Y%m%d`.state

If something went wrong, you can redownload the packages you had installed on
that day. Use --debs to download all binaries that you had installed for one or
more given source packages:

    debcya --state=20160106.state --debs network-manager

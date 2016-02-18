# ableton-experiment
The great Ableton + git experiment.

Attempting to discover what we can and can't do with Ableton + git in the context of many collaborators on one .als file.

Article: link to come

##Setup:

Ensure gzip/zcat is installed. If you have [GitHub Desktop](https://desktop.github.com/) with its git bash installed, I believe that should be sufficient.

Then run:

    git config filter.zcat.smudge "zcat -f"
    git config filter.zcat.clean "zcat -f"

In combination with the .gitattibutes file in this project, this will tell git to keep .als files "never not unzipped." git will attempt to keep your .als files unzipped, but Ableton will compress them on save. Unzipped versions will come out of git when you checkout.

##Remember:

 * Collect All and Save!
 * Don't commit DLLs! If you use VSTs, use free ones and add a link to download in file vsts.md!
 * The golden rule of collaboration: Be bold!

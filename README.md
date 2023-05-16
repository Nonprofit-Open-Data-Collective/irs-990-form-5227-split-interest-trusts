# irs-990-form-5227-split-interest-trusts
R scripts to document and build the IRS Current Exempt Organizations Database.

From: https://www.irs.gov/charities-non-profits/exempt-organizations-business-master-file-extract-eo-bmf

Split Interest Trust Data collected from Forms 5227, Split-Interest Trust Information Returns.

```r
library( tidyverse )

d.2020 <- read_csv( "https://www.irs.gov/pub/irs-soi/sit-2020.csv" )
d.2019 <- read_csv( "https://www.irs.gov/pub/irs-soi/2019-sit.csv" )
d.2018 <- read_csv( "https://www.irs.gov/pub/irs-soi/2018_sit.csv" )
d.2017 <- read_csv( "https://www.irs.gov/pub/irs-soi/SIT%202017.csv" )
d.2016 <- read_csv( "https://www.irs.gov/pub/irs-soi/SIT%202016.csv" )


```

## [Split-Interest Trusts](https://www.irs.gov/charities-non-profits/private-foundations/split-interest-trusts)

A split-interest trust is a trust that:

* Is not exempt from tax,
* Has some unexpired interests that are devoted to purposes other than religious, charitable, or similar purposes described in Internal Revenue Code section 170(c)(2)(B), and
* Has amounts in trust for which a char­itable contribution deduction has been allowed.

Also included under these provisions is a split-interest trust that is not treated as a charitable trust during a reasonable period of settle­ment or while it is winding up.

A split-interest trust is subject to the following provisions in the same manner as is a private foundation:

* Terminations, both voluntary and involuntary. Note, though, that the termination rules do not apply to certain payments by split interest trusts.
* Governing instruments,
* Tax on self-dealing,
* Tax on excess business holdings,
* Tax on investments that jeopardize chari­table purposes, and
* Tax on taxable expenditures.

These provisions do not apply to amounts transferred in trust before May 27, 1969.

The taxes on excess business holdings and on jeopardizing investments do not apply if the income interest of a trust and none of the remainder interest is devoted to charitable purposes; a charitable deduction was allowed; and those interests for which a charitable deduction was allowed have an aggregate fair market value of all amounts in trust. Also, these two taxes do not apply if a charitable deduction was allowed for amounts payable under the terms of the trust to every remainder beneficiary and none of the income beneficiaries.

The taxes on self-dealing and taxable expenditures do not apply to any amounts payable under the terms of a split-interest trust to income beneficiaries, unless a chari­table contribution deduction was allowed with respect to the income interest of the beneficiary. For example, Hyram Jones created a split-interest trust that is required annually to pay Melanie Jones 5 percent of the net fair market value of the trust assets, valued annually, for her life; and to pay the remainder to Y, a section 501 (c)(3) organi­zation. A charitable contribution deduction was allowed for the remainder interest. Each annual amount payable to Melanie for her life is not subject to the provisions listed earlier. These payments are not acts of self-dealing or taxable expenditures. However, with the exception of the income interest so paid, the trust is subject to the provisions in the same manner as if the trust were a private foundation.

Also not included are certain amounts segregated for charitable purposes.

Additional information: See Revocable trusts that become split-interest trusts

-----------

A split-interest trust will continue to be treated as a split-interest trust until the date final distribution of all the net assets is made, if all of the following conditions are met:

* All unexpired interests in the trust are charitable remainder interests.
* All charitable beneficiaries have become entitled to distributions of corpus in trust or free of trust.
If, however, after any intervening interests expire, the trust is considered terminated for federal income tax purposes, the trust will then be treated as a charitable trust rather than a split-interest trust between the date on which the trust is considered terminated and the date final distribution of all the net assets is made.  These provisions do not affect the determination of the tax liability of the beneficiaries of the trusts. 

Split-interest trusts that become charitable trusts.  A split-interest trust in which all of the unexpired interests are charitable remainder interests and in which charitable beneficiaries are not entitled to distributions of corpus will continue to be treated as a split-interest trust for a reasonable period of settlement after noncharitable interest expires.  A split-interest trust that under its terms is to continue to hold assets for charitable beneficiaries after the noncharitable interest expires rather than distributing them is allowed a reasonable period of time for settlement before being treated as a charitable trust.

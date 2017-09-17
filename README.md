# BC Badge

# Introduction
This repository is used to keep the Berau Coal's ID card preview. There are several types of ID card, including:
* ID Card which applicable for Employees, Contractors, Subcontractors, Study.
* Guest ID Card which applicable for Temporary Workers and Visitors.
* SIMPER which applicable for Employees, Contractors and Subcontractors.
* KIMPER which applicable for Employees, Contractors and Subcontractors.
* Land Clearing.
* Dumping Operator.
* Transhipment Access Card.

# Project Directory
* `/asset` - keep logo, font and other assets.
* `/css` - css files, separated into different css files for each type.
* `index.html` - preview of ID Card.

# Badges
## ID Card
### Code
```html
<div class="badge badge--id">
   <div class="badge__header">
       <div class="header__company">
           <img src="asset/berau-logo.svg"> ** Replace with company logo.
       </div>
       <div class="header__type">
          <div class="type__title">
              <p>ID CARD</p>
          </div>
          <div class="type__subtitle">
              <p>KARYAWAN</p> ** Replace with other ID Card subtype, i.e. Kontraktor, Subkontraktor, etc.
          </div>
       </div>
    </div>
    <div class="badge__body">
       <img class="user__picture" src="http://www.saparch.com/public/widget/1_widget_john-doe.png"> ** Replace with user Image.
    </div>
    <div class="badge__footer">
       <h3 class="user__name">Heru Sukoco</h3> ** Replace with user name.
       <p class="user__label">BMO1-123</p> ** Replace with NIK.
       <p class="website">www.beraucoal.co.id</p>
    </div>
</div>
```
## Guest Card
### Code
```html
<div class="badge badge--guest">
    <div class="badge__header">
        <div class="header__company">
            <img src="asset/berau-logo.svg"> ** Replace with company logo.
        </div>
        <div class="header__type">
            <div class="type__title">
                <p>ID CARD</p>
            </div>
        </div>
    </div>
    <div class="badge__body">
        <p class="guest__company">PT. Nama Perusahaan</p> ** Replace with company name, or add "hidden" class to hide it.
        <h3 class="guest__number guest__number--visitor">001</h3> ** Replace with 3 digits number.
    </div>
    <div class="badge__footer">
        <p class="label">VISITOR</p> ** Replace with guest type, i.e.: Temporary Worker or Visitor.
        <p class="website">www.beraucoal.co.id</p>
    </div>
</div>
```
## Land Clearing Operators Card
### Code
```html
<div class="badge badge--lc">
    <div class="badge__header">
        <div class="header__company">
            <img src="asset/berau-logo.svg"> ** Replace with company logo.
        </div>
        <div class="header__ministry">
            <img src="asset/esdm-logo.svg"> ** Replace with ministry logo.
        </div>
    </div>
    <div class="badge__body">
        <h3 class="lc__title">Kartu Pengawas Operasional Land Clearing</h3> ** Replace with ministry functions.
        <img class="lc__picture" src="http://www.saparch.com/public/widget/1_widget_john-doe.png"> ** Replace with user picture.
        <p class="lc__name">Nama Petugas</p> ** Replace with user name.
    </div>
    <div class="badge__footer">
        <table class="remarks">
            <tbody>
            <tr>
                <td>No Reg</td>
                <td>:</td>
                <td>{{No Reg}}</td> ** Replace with registry number.
            </tr>
            <tr>
                <td>NPK</td>
                <td>:</td>
                <td>{{NPK}}</td> ** Replace with NPK.
            </tr>
            <tr>
                <td>Perusahaan</td>
                <td>:</td>
                <td>{{Perusahaan}}</td> ** Replace with company name.
            </tr>
            <tr>
                <td>Masa Berlaku</td>
                <td>:</td>
                <td>{{Masa Berlaku}}</td> ** Replace with valid period.
            </tr>
            </tbody>
        </table>
        <p class="website">www.beraucoal.co.id</p>
    </div>
</div>
```
## Dumping Operator Card
### Code
```html
<div class="badge badge--dm">
    <div class="badge__header">
        <div class="header__company">
            <img src="asset/berau-logo.svg"> ** Replace with company logo.
        </div>
        <div class="header__ministry">
            <img src="asset/esdm-logo.svg"> ** Replace with ministry logo.
        </div>
    </div>
    <div class="badge__body">
        <h3 class="dm__title">Kartu Petugas<br>Dumping</h3> ** Replace with ministry function.
        <img class="dm__picture" src="http://www.saparch.com/public/widget/1_widget_john-doe.png"> ** Replace with user picture.
    </div>
    <div class="badge__footer">
        <table class="remarks">
            <tbody>
            <tr>
                <td>No Reg</td>
                <td>:</td>
                <td>{{No Reg}}</td> ** Replace with registry number.
            </tr>
            <tr>
                <td>Nama</td>
                <td>:</td>
                <td>{{Nama}}</td> ** Replace with user name.
            </tr>
            <tr>
                <td>NPK</td>
                <td>:</td>
                <td>{{NPK}}</td> ** Replace with NPK.
            </tr>
            <tr>
                <td>Perusahaan</td>
                <td>:</td>
                <td>{{Perusahaan}}</td> ** Replace with company.
            </tr>
            <tr>
                <td>Masa Berlaku</td>
                <td>:</td>
                <td>{{Masa Berlaku}}</td> ** Replace with validity period.
            </tr>
            </tbody>
        </table>
        <p class="penalty-title">Pelanggaran</p>
        <table class="penalty">
            <tr>
                <td>1</td>
                <td>2</td>
                <td>3</td>
            </tr>
        </table>
    </div>
</div>
```
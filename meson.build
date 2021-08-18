# project naem
project('com.github.NRDsstuff.gtk-helo-again', 'vala', 'c')

# create a new exe
executable(
    meson.project_name(),
    'src' / 'Application.vala',
    dependencies:[
        dependency('gtk+-3.0')
    ],
    install: true
)

# install the .desktop
install_data(
    'data' / 'dumb.desktop',
    install_dir: get_option('datadir') / 'applications',
    rename: meson.project_name() + '.desktop'
)

# xml lul
install_data(
    'data' / 'helo-again.appdata.xml',
    install_dir: get_option('datadir') / 'metainfo',
    rename: meson.project_name() + '.appdata.xml'
)
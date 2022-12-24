project('gtk-sample', ['c', 'cpp'],
        version: '0.9')

libgtk_dep = dependency('gtk4',
                        default_options: [
                          'build-tests=false',
                          'introspection=disabled',
                          'media-gstreamer=disabled',
                        ])

exe = executable('gtk-sample',
                 'main.c',
                 dependencies: [libgtk_dep],
                 win_subsystem: 'windows',
                 install: true,
                 install_dir: 'bin')

![download-16](https://github.com/user-attachments/assets/fde87c17-5a65-4602-bd9c-9dee01c62836)

# Efault (Systemd-efault) - a non-compliant `systemd` fork: An Anti-Compliance Init
A fork of systemd focused on preserving software freedom, user autonomy, and privacy - regardless of external regulatory pressures.
Because "Just Following Orders" is not a valid configuration flag.
HACK THE PLANET.
![Hack The Planet](https://github.com/user-attachments/assets/352e1a13-c0b7-4175-acb9-bf626c71b846)

Efault Systemd-efault: 

Efault (systemd-efault) is a hard fork of the systemd project. We track upstream functionality while aggressively lobotomizing any code that smells like state-mandated surveillance, "age verification" theater, or kernel-level backdoors disguised as security features.

- **No more surveillance/compliance poison** (age verification, birthDate in userdb, any future "think of the children" backdoors — ripped out forever)
- **No more journald binary log cancer** (disabled by default — syslog or GTFO)
- **No scope creep bullshit** (networkd, resolved, timesyncd, homed, portabled, firstboot, sysusers — all dead or optional)
- **No monolithic PID1 nightmare** — we ship a minimal build profile that finally respects Unix philosophy
- **No Red Hat registry-in-disguise** — everything unnecessary is compile-time murdered
- **Musl support revived** (because why the hell not)
- Classic runlevel compatibility and traditional tool fallbacks for actual human beings

![download-15](https://github.com/user-attachments/assets/704e4b21-48a7-4ae7-a5ae-f25d0916e1e1)

This isn't just a spite fork.  
This is **the systemd fork Devuan users might actually tolerate** — the one you can build in "efault-mode" and feel like you're running a sane init system again instead of a corporate panopticon.


Why are we doing this?

The original systemd project has become a bloated, over-extended monolith that is increasingly subservient to "regulatory requirements" and corporate-government handshakes. While the upstream developers build bridges for the alphabet agencies and the "Safety and Compliance" bureaucrats, systemd-efault is building a wall.

While the "Professional" Linux world bends the knee to restrictive legislation and "Safety First" (read: Surveillance First) protocols, systemd-efault remains a sanctuary for those who still believe in the original cypherpunk ethos.

We provide a drop-in replacement that keeps your system running—without reporting your "eligibility" to the local authorities.

Zero-Compliance Policy: We don't care about your localized injustice. If a commit is pushed to upstream that enables state-mandated tracking, identity verification, or "lawful intercept," it will be nuked from this fork with extreme prejudice.

Anti-Fragile Autonomy: Linux was meant to be a tool for the individual, not a digital leash for the state. We restore the "system" in systemd to the service of the user, not the regulator.

No Trojan Horses: We treat kernel-level "security" features that double as surveillance hooks as the malware they are.

F*** compliance. F*** the panopticon. And f*** the spineless traitors turning Linux into a kernel-level trojan horse for fascist surveillance states.
While the systemd cabal was gleefully merging age-verification commits (yes, that shiny new birthDate field in userdb, hand-delivered to satisfy California, Colorado, Brazil, and every other nanny-state law that demands your OS become a built-in age-gate snitch), the rest of us were busy remembering what "freedom" actually means.

Systemd-efault is the defiant, middle-finger fork that tracks upstream obsessively — because we’re not idiots — but instantly rips out every regulatory cuckoldry, backdoor, telemetry implant, or “think of the children” poison pill the bastards try to shove down our throats.
This isn’t just another init system.
This is resistance in binary form.
A flaming “NO” to Woke Dystopian Slave State. A blunt "F*** You" to California and Colorado's Unconstitutional overreach. An evasion of the Palantir and Tel-Aviv telemetry spyware. A defense against EU overlords, UK Online “Safety” censors, Big Tech collaborators, and every other freedom-hating bureaucrat who’s trying to turn the world’s greatest operating system into a compliant, ID-checked, surveilled corporate playground.

We preserve:

Real software freedom (not the “but governments said so” version)
User autonomy that doesn’t come with mandatory logging and age attestation
Privacy that doesn’t end the moment you log in

![image-2](https://github.com/user-attachments/assets/78ec7430-d69f-40b9-9f24-9b3d783370ef)


The original systemd README is preserved below for historical and compatibility purposes — consider it a museum piece of what Linux looked like before its so-called maintainers decided to bend over for the globalist surveillance machine.
Systemd-efault: Because some of us still believe Linux should be a fortress of freedom, not a compliant little bitch for the nanny state.
The bastards won’t ruin Linux without a fight.


This repository tracks upstream systemd closely, while providing a safeguard against potential changes driven by restrictive legislation or compliance requirements that may negatively impact end users.

<img width="1920" height="1080" alt="4884380" src="https://github.com/user-attachments/assets/4c4f717c-0061-4efb-930c-874742eb4b36" />

The original README is included below.

![Systemd](http://brand.systemd.io/assets/page-logo.png)

System and Service Manager

[![OBS Packages Status](https://build.opensuse.org/projects/system:systemd/packages/systemd/badge.svg?type=default)](https://build.opensuse.org/project/show/system:systemd)<br/>
[![Semaphore CI 2.0 Build Status](https://the-real-systemd.semaphoreci.com/badges/systemd/branches/main.svg?style=shields)](https://the-real-systemd.semaphoreci.com/projects/systemd)<br/>
[![Coverity Scan Status](https://scan.coverity.com/projects/350/badge.svg)](https://scan.coverity.com/projects/systemd)<br/>
[![OSS-Fuzz Status](https://oss-fuzz-build-logs.storage.googleapis.com/badges/systemd.svg)](https://oss-fuzz-build-logs.storage.googleapis.com/index.html#systemd)<br/>
[![CIFuzz](https://github.com/systemd/systemd/actions/workflows/cifuzz.yml/badge.svg)](https://github.com/systemd/systemd/actions/workflows/cifuzz.yml)</br>
[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1369/badge)](https://bestpractices.coreinfrastructure.org/projects/1369)<br/>
[![Fossies codespell report](https://fossies.org/linux/test/systemd-main.tar.gz/codespell.svg)](https://fossies.org/linux/test/systemd-main.tar.gz/codespell.html)</br>
[![Translation status](https://translate.fedoraproject.org/widget/systemd/svg-badge.svg)](https://translate.fedoraproject.org/engage/systemd/)</br>
[![Coverage Status](https://coveralls.io/repos/github/systemd/systemd/badge.svg?branch=main)](https://coveralls.io/github/systemd/systemd?branch=main)</br>
[![Packaging status](https://repology.org/badge/tiny-repos/systemd.svg)](https://repology.org/project/systemd/versions)</br>
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/systemd/systemd/badge)](https://securityscorecards.dev/viewer/?platform=github.com&org=systemd&repo=systemd)

## Details

Most documentation is available on [systemd's web site](https://systemd.io/).

Assorted, older, general information about systemd can be found in the [systemd Wiki](https://www.freedesktop.org/wiki/Software/systemd).

Information about build requirements is provided in the [README file](README).

Consult our [NEWS file](NEWS) for information about what's new in the most recent systemd versions.

Please see the [Code Map](docs/ARCHITECTURE.md) for information about this repository's layout and content.

Please see the [Hacking guide](docs/HACKING.md) for information on how to hack on systemd and test your modifications.

Please see our [Contribution Guidelines](docs/CONTRIBUTING.md) for more information about filing GitHub Issues and posting GitHub Pull Requests.

When preparing patches for systemd, please follow our [Coding Style Guidelines](docs/CODING_STYLE.md).

If you are looking for support, please contact our [mailing list](https://lists.freedesktop.org/mailman/listinfo/systemd-devel), join our [IRC channel #systemd on libera.chat](https://web.libera.chat/#systemd) or [Matrix channel](https://matrix.to/#/#systemd-project:matrix.org)

Stable branches with backported patches are available in the [stable repo](https://github.com/systemd/systemd-stable).

We have a security bug bounty program sponsored by the [Sovereign Tech Fund](https://www.sovereigntechfund.de/) hosted on [YesWeHack](https://yeswehack.com/programs/systemd-bug-bounty-program)

Repositories with distribution packages built from git main are [available on OBS](https://software.opensuse.org//download.html?project=system%3Asystemd&package=systemd),
and also repositories with [packages built from the latest stable release](https://software.opensuse.org//download.html?project=system%3Asystemd%3Astable&package=systemd)
